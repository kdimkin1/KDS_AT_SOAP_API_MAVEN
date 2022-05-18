# Automation Tests (run SOAP-API tests from SoapUI project)

## Technology Stack
| <a href="https://www.jetbrains.com/idea/"><img src="https://starchenkov.pro/qa-guru/img/skills/Intelij_IDEA.svg" width="40" height="40"  alt="IDEA"/></a> | <a href="https://www.jetbrains.com/idea/"><img src="https://starchenkov.pro/qa-guru/img/skills/Java.svg" width="40" height="40"  alt="Java"/></a> | <a href="https://www.jetbrains.com/idea/"><img src="https://upload.wikimedia.org/wikipedia/commons/5/52/Apache_Maven_logo.svg" width="60" height="40"  alt="maven-logo"/></a> | <a href="https://www.jetbrains.com/idea/"><img src="https://www.ph4.org/_RU/DL/LOGO/s/soapui.gif" width="100" height="40"  alt="SoapUI"/></a> |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------:| :---------: |:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------:|
|                                                                           IDEA                                                                            | Java |                                                                                     Maven                                                                                     |                                                                    SoapUI                                                                     |

Run command:

```bash
mvn com.smartbear.soapui:soapui-maven-plugin:5.0.0:test
```

See details:
```bash
SoapUI project example with some tests for SOAP local service:
../soap-ui-example_hw_4maven_plagin.xml

```
Common links:
```bash
Local SOAP service
https://github.com/spring-guides/gs-producing-web-service
https://spring.io/guides/gs/producing-web-service/
Note:
1. If use Java > 8 add to build.gradle:
    implementation 'javax.xml.bind:jaxb-api:2.3.0'
    implementation 'javax.activation:activation:1.1'
    implementation 'org.glassfish.jaxb:jaxb-runtime:2.3.0'
2. Use Jaxb for generate models by xsd scheme 
cd complete
gradle genJaxb 
3. Run with main() from ProducingWebServiceApplication.class: 
4. Check: http://localhost:8080/ws/countries.wsdl

SoapUI Documentation (should use VPN if not available):
https://www.soapui.org/docs/test-automation/maven/maven-2-x/
SoapUI plagin repositorys:
http://www.soapui.org/repository/maven2/
https://rapi.tools.ops.smartbear.io/nexus/content/groups/public/


Plagin for gradle: 
https://daggerok.github.io/soapui-runner/#frequently-asked-questions
```

