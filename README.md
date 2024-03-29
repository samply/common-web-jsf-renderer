# JSF Bootstrap Message and Messages Renderer


Style the h:messages component from JSF with [bootstrap alerts](https://getbootstrap.com/docs/3.3/components/#alerts)


Use maven to build the jar:

```
mvn clean install
```

In order to use it in any JSF2 project:

* Bootstrap has to be included in the project
* Add the following snippet to _faces-config.xml_:

   ```xml
   <!-- Register the custom renderers to use bootstrap message(s) -->
   <render-kit>
       <renderer>
           <component-family>javax.faces.Message</component-family>
           <renderer-type>javax.faces.Message</renderer-type>
           <renderer-class>de.samply.share.client.renderer.BootstrapMessageRenderer</renderer-class>
       </renderer>
       <renderer>
           <component-family>javax.faces.Messages</component-family>
           <renderer-type>javax.faces.Messages</renderer-type>
           <renderer-class>de.samply.share.client.renderer.BootstrapMessagesRenderer</renderer-class>
       </renderer>
   </render-kit>
 ```

 ## License
        
 Copyright 2020 The Samply Development Community
        
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
        
 http://www.apache.org/licenses/LICENSE-2.0
        
 Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
 
