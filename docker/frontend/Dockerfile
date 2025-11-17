FROM node:20.18.0-alpine

RUN apk update
RUN apk add python3-dev bash make g++ tzdata
ENV NODE_OPTIONS="--max-old-space-size=2048"

RUN mkdir /nuxt
ADD . /nuxt
WORKDIR /nuxt

RUN yarn global add pm2
RUN pm2 install pm2-logrotate && \
    pm2 set pm2-logrotate:retain 20 && \
    pm2 set pm2-logrotate:max_size 100M && \
    pm2 set pm2-logrotate:compress false && \
    pm2 set pm2-logrotate:copytruncate true && \
    pm2 set pm2-logrotate:rotateInterval "0 0 * * *"

CMD ["pm2-runtime", "start", "pm2.config.js"]
