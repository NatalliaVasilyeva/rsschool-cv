# __Java Developer CV__
---

## __Contacts:__
---

* telephone number: +375-29-501-52-96 (MTS, Viber, Telegram);
* email: nn1.vasilyeva@gmail.com;
* skype: vasnatnik;
* github: https://github.com/NatalliaVasilyeva

## __Summary:__
---

I already have programming knowledge in Java, SQL, C# and a little bit in JS.  And now I want to study new programming language for Android development. 

## __Skills:__
---

- Java
- C#
- Spring (SpringBoot, Spring-mvc, Spring-jdbc ...)
- REST API
- Maven
- Hibernate
- MySQL
- JPA
- JSP
- JUnit
- Mockito
- TomCat
- CSS/HTML/JS
- XML
- XSTL
- Git
- Jira
- Confluence

## __Code example:__
---

```
public void run() {
        try {
            InputStream inputStream = socket.getInputStream();
            BufferedReader reader = new BufferedReader(new InputStreamReader(inputStream, StandardCharsets.UTF_8));
            while (!socket.isClosed()) {
                String message = reader.readLine();
                ChatMessage json= MessageServiceImpl.INSTANCE.parseFromJson(message);
                if (json != null) {
                    if (user == null || user.isUserExit()) {
                        user = UserServiceSingleton.INSTANCE.registerUser(json);
                        user.setSocket(socket);
                        user.setType(UserType.CONSOLE);
                        UserServiceSingleton.INSTANCE.addUserToCollections(user);
                        continue;
                    } else
                   CommandFactory commandFactory = new CommandFactory(user);
                    commandFactory.startCommand(json);
                }
            }
        } catch (IOException e) {
            UserServiceSingleton.INSTANCE.exitUser(user);
            user.disconnectUserByServer();
            LOGGER.error("Problem with reading message  " + e.getMessage());
        }
    }
```
---

## __Experience:__
---

09.2019-now:
 Junior java developer in product company. Write code on Java 8, 11, fix defects, write unit and functional tests for new functional

03.2006-09.2019:
 Accountant, chief accountant