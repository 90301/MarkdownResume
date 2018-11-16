# Java / JEE (Java Enterprise Edition)
Started : 2009

# Projects Utilizing Java / Java EE

## [Blue Chip AI](https://bluechipai.net/)
Blue Chip AI uses Java for all internal projects to take advantage of Java's Parallel Stream Performance, 
often times outperforming all low level language implementations thanks to the advancements in Just In Time (JiT) compiling.

The ease of *Vaadin* integration for all user interfaces allows us to focus more on the Artificial Intelligence, while not compromising on a user interface (UI).

## [Style Connect](https://90301.github.io/StyleConnectWebsite/)
Style Connect is an [Open Source](https://github.com/90301/Crescent-CRM-V/tree/Release/Crescent-CRM-Vaadin-Maven) CRM Software for Salons, utilizing Social Media Data Mining Techniques combined with AI for Analysis, 
you can know your clients **better then they know themselves.** 

Style connect uses Java EE to power the Vaadin interface that runs the application. 

<img src="https://user-images.githubusercontent.com/6025683/48597927-580fd480-e92e-11e8-99f1-f6034968929f.png">

## Multi-Agent / Economic Simulations
Understanding how economies function at both a macro and micro level usually requires building a model, 
With a **Multi-Agent** simulation, you are able to simulate at the individual level, but see effects up to the macro level. 
These insights are particularly helpful when attempting to understand if a particular theory works correctly.

Java **Stream processing** performance helps ensure highly parallel runtimes execute optimally. Java allows easy deployment to
**super computers.** 

Some of these simulations have a graphical component to them (though most do not).

<img src="https://raw.githubusercontent.com/90301/Boats/UI1/Command%20Links%20whirlpool%20patteren.png">


# Related Languages

### [C#](https://github.com/90301/MarkdownResume/blob/master/Technologies/C_Sharp.md)
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
| Servers | Frameworks | Management | Continuous Integration | 
|---------|------------|-------|----------------------------|
| Tomcat | Vaadin | Apache Maven | Jenkins |
| Glassfish | Spring | Apache Ivy  | |
| JBoss | | Apache Ant | |

## Don't see your server here?
In general, Java EE works identically across servers. Simply deploy the .WAR file to the server. 
From a development standpoint there is no difference between using any type of Java EE web server.

## Why would you use these servers?
In order to keep costs low for organizations, it is advised to use Tomcat for low / medium load applications. 
When clustering is needed, JBoss or Glassfish work well with clustering and the setup is a breeze.
