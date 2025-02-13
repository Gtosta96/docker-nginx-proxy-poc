FROM node:20.12.2 AS react_builder
COPY . /code/
WORKDIR /code

FROM nginx
RUN rm -rf /usr/share/nginx/html/*
COPY --from=react_builder /code/build /usr/share/nginx/html/react/
COPY --from=react_builder /code/storybook-static /usr/share/nginx/html/react/storybook-static/