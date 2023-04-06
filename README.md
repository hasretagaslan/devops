   ### spring-mongo-docker-compose-crud(GET-POST-PUT)
*Proje Spring boot ve MongoDB kullanarak oluşturalan Rest Api uygulamasının CRUD İşlemlerini docker-compose ile docker container ayağa kaldırarak çalıştırır.*

*Docker Compose, çok konteynerli Docker uygulamasını çalıştırır. Yapılandırma dosyasını okuyarak tek bir docker-compose komutu ile birden çok docker container çalıştırmamızı sağlar. Bu projede (Mongo container ve Spring boot uygulamasını kulanan RestApi containeri var).*

  **Java** 
  
  **Spring Boot** 
  
  **Mongo DB**
  
  **Docker**
  
   **Docker-compose**
  
   **IntelliJ IDEA** 
 
   **Postman**
  
### Uygulamayı oluşturun ve çalıştırın

docker-compose.yml dosyası, ortamı yapılandırmak için gerekli tüm ayarları içerir. 

Terminalinizde Projeyi indirdiğiniz klasöre gelip

              docker-compose up -d
  
  komutunu çalıştırıp ardından
  
 Docker compose dosyasına verileri ekeyemediğim için ardından bu komutu ekleyip verilerimizi containera ekliyoruz.
 
              docker exec mongodb  mongoimport -d test -c test --type csv --file /home/London.csv --headerline
  
 ###  APİ Belgeleri
 
 [GET:] http://localhost:8080/findAllHouse
 
 [POST:] http://localhost:8080/addNewHouse
 
 [PUT:] http://localhost:8080/updateHouse/{id}
 
Postman kullanarak bu adreslerde test edebilirsiniz.

 *Son olarak*
 
               docker-compose down 
               
  Containeri durdurabiliriz.
