# 1. Java environment
FROM eclipse-temurin:17-jdk

# 2. Work directory
WORKDIR /app

# 3. Saari files copy karo
COPY . .

# 4. Bin folder banao aur compile karo
RUN mkdir -p bin
RUN javac -d bin src/Main.java src/com/waste/service/*.java

# 5. Port expose (Render dynamic port use karega, par hum 8080 define kar rahe hain)
EXPOSE 8080

# 6. Run the application
CMD ["java", "-cp", "bin", "Main"]
