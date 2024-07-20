FROM openjdk:11-jdk
WORKDIR /app
COPY target/your-application.jar app.jar
COPY lib/ojdbc8.jar /app/lib/
COPY lib/postgresql.jar /app/lib/
EXPOSE 8080
ENV ORACLE_URL=jdbc:oracle:thin:@oracle-host:1521/your_service_name
ENV ORACLE_USER=your_oracle_username
ENV ORACLE_PASSWORD=your_oracle_password
ENV POSTGRES_URL=jdbc:postgresql://postgres-host:5432/your_database
ENV POSTGRES_USER=your_postgres_username
ENV POSTGRES_PASSWORD=your_postgres_password
CMD ["java", "-cp", "app.jar:/app/lib/*", "com.yourcompany.YourMainClass"]