FROM openjdk:8-jdk

# Set environment variables for Android SDK
ENV ANDROID_HOME /usr/local/android-sdk
ENV PATH ${PATH}:${ANDROID_HOME}/tools:${ANDROID_HOME}/platform-tools

RUN wget -q "https://dl.google.com/android/repository/sdk-tools-linux-4333796.zip" -O android-sdk.zip \
    && unzip android-sdk.zip -d $ANDROID_HOME \
    && rm android-sdk.zip

RUN yes | $ANDROID_HOME/tools/bin/sdkmanager --licenses

# Install Android Build Tools and libraries
RUN $ANDROID_HOME/tools/bin/sdkmanager "platform-tools" "platforms;android-28" "build-tools;28.0.3"

WORKDIR /usr/src/app

COPY . .

CMD ["./gradlew", "assemble"]
