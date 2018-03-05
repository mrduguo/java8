FROM openjdk:8
ENTRYPOINT ["java", "-jar", "/app.jar"]
EXPOSE 8080

#https://stackoverflow.com/questions/34110426/does-java-support-lets-encrypt-certificates
RUN wget https://letsencrypt.org/certs/lets-encrypt-x3-cross-signed.der && \
    keytool -trustcacerts -keystore \$JAVA_HOME/jre/lib/security/cacerts -storepass changeit -noprompt -importcert -alias lets-encrypt-x3-cross-signed -file lets-encrypt-x3-cross-signed.der && \
    rm -f lets-encrypt-x3-cross-signed.der
