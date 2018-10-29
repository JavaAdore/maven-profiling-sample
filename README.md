# maven-profiling-sample
Just sample implementation to build maven project as per environemnt

populate properties values for /src/main/resources/envrionment.properties

for example mvn clean install -P development

file /src/main/resources/envrionment.properties has a property called current.environment=${current.environment} ${current.environment} will be replaced to the associated value with key ${current.environment} in /src/main/resources/profiles/development/environment.properties and so on for other profiles (test,staging,production)
