# Java / JEE (Java Enterprise Edition)
Start : 2009

# Projects Utilizing Java

# Related Languages

### C#
C# shares nearly the exact same design / development paradigms. Stream processing has the same performance and functionality, just with different method names.

To demonstrate that, here's some example code calculating the total sales made in a given year between the two languages.
```C#
//C#
List<Sales> list = new List<>();
//...
Double totalSales = list.stream()
.Select(x -> x.getSalePrice())
.Aggregate((x,y) -> x + y);

```

```Java
//Java
List<Sales> list = new ArrayList<>();
//...
Double totalSales = list.stream()
.map(x -> x.getSalePrice())
.reduce((x,y) -> x + y).orElse(0.0);
```

Both of these examples do the exact same thing, the two languages even share the same syntax. 

# Technology
| Servers | Frameworks |
|---------|------------|
| Tomcat | Vaadin |
| Glassfish | Spring |
| JBoss | |

## Don't see your server here?
In general, Java EE works identically across servers. Simply deploy the .WAR file to the server. 
From a development standpoint there is no difference between using any type of Java EE web server.

## Why would you use these servers?
In order to keep costs low for organizations, it is advised to use Tomcat for low / medium load applications. 
When clustering is needed, JBoss or Glassfish work well with clustering and the setup is a breeze.