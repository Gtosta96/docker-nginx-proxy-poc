FROM node:20.12.2 AS builder
COPY . /code/
WORKDIR /code

FROM nginx
RUN rm -rf /usr/share/nginx/html/*
COPY --from=builder /code/dist /usr/share/nginx/html/