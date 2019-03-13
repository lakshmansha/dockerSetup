#  Create a new image from the android-setup:v1 for android build image.
FROM android-setup:latest

#Display the Android Dependencies
RUN printenv

RUN echo " Installing Node & Npm "

#Install Node.
RUN curl https://nodejs.org/dist/v10.15.0/node-v10.15.0-linux-x64.tar.gz | tar xz -C /usr/local/ --strip=1

# Update npm package.
RUN npm install npm@latest -g

RUN echo " Node & NPM Installation Completed "

RUN echo " Installing Cordova Dependencies "

# Install cordova package.
RUN npm install cordova -g

# Install Ngx-Scripts package.
RUN npm install @ngx-rocket/scripts -g

# Install Ngx-Scripts package.
RUN npm install gulp -g

# Install Ngx-Scripts package.
RUN npm install bower -g

RUN echo " Cordova Dependencies Installation Completed "

# Start the application. This is the same as running ng start.
CMD ["npm", "run", "docker"]