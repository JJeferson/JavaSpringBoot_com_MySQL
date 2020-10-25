# JavaSpringBoot_com_MySQL
Dependências e exemplo


# Dependencias, elas devem ser declaradas dentro do pom.xml

		
                		            <dependency>
		                           	<groupId>org.springframework.boot</groupId>
			                          <artifactId>spring-boot-starter-data-jpa</artifactId>
		                            </dependency>
		                            <dependency>
			                          <groupId>org.springframework.boot</groupId>
			                          <artifactId>spring-boot-starter-data-rest</artifactId>
	                            	</dependency> 
		                 
                            		<dependency>
	                          		<groupId>mysql</groupId>
	                          		<artifactId>mysql-connector-java</artifactId>
		                           	<scope>runtime</scope>
	                            	</dependency>

# Depois disso dentro do aplication.properties

                                 spring.jpa.properties.jdbc.lob.non_contextual_creation=true

                                 #Banco local = jcommerce
                                 spring.datasource.url= jdbc:mysql://endereço:porta/nome_do_Banco_de_dados?useTimezone=true&serverTimezone=UTC
                                 spring.datasource.username=User do seu banco de dados mysql
                                 spring.datasource.password= senha
                                 spring.jpa.hibernate.ddl-auto=update
                                 
                                 
# É importante que seja desta forma para que o backend faça a gestão do seu banco de dados, criando e editando tabelas quando precisar.                                 
