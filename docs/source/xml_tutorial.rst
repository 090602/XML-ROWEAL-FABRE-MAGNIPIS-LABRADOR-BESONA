<?xml version="1.0" encoding="UTF-8"?>
<xml_tutorial>
    <section title="XML HOME">
        <content>Introduction to XML and its importance in data storage and transfer.</content>
        <example><![CDATA[
            <note>
                <to>Tove</to>
                <from>Jani</from>
                <message>Hello, XML!</message>
            </note>
        ]]></example>
    </section>
    <section title="XML Introduction">
        <content>Explains XML (eXtensible Markup Language) as a flexible text format for structuring data.</content>
        <example><![CDATA[
            <?xml version="1.0"?>
            <bookstore>
                <book>
                    <title>XML Guide</title>
                    <author>John Doe</author>
                    <price>29.99</price>
                </book>
            </bookstore>
        ]]></example>
    </section>
    <section title="XML How to use">
        <content>Guides on using XML in various applications like web services, databases, and configurations.</content>
        <example><![CDATA[
            <config>
                <setting name="theme" value="dark"/>
                <setting name="language" value="en"/>
            </config>
        ]]></example>
    </section>
    <section title="XML Tree">
        <content>Shows the hierarchical structure of XML documents with elements and nesting.</content>
        <example><![CDATA[
            <family>
                <parent>
                    <child name="Alice"/>
                    <child name="Bob"/>
                </parent>
            </family>
        ]]></example>
    </section>
    <section title="XML Syntax">
        <content>Describes XML syntax rules such as case sensitivity, proper nesting, and closing tags.</content>
        <example><![CDATA[
            <person>
                <name>John</name>
                <age>30</age>
            </person>
        ]]></example>
    </section>
    <section title="XML Elements">
        <content>Defines XML elements as the building blocks of an XML document.</content>
        <example><![CDATA[
            <car>
                <make>Toyota</make>
                <model>Corolla</model>
            </car>
        ]]></example>
    </section>
    <section title="XML Attributes">
        <content>Explains attributes in XML to add metadata to elements.</content>
        <example><![CDATA[
            <user id="123" name="Alice" role="admin"/>
        ]]></example>
    </section>
    <section title="XML Namespaces">
        <content>Demonstrates how namespaces prevent element name conflicts in XML documents.</content>
        <example><![CDATA[
            <root xmlns:book="http://example.com/book">
                <book:title>XML Basics</book:title>
            </root>
        ]]></example>
    </section>
    <section title="XML Display">
        <content>Describes methods to display XML data using CSS and XSLT.</content>
        <example><![CDATA[
            <?xml-stylesheet type="text/css" href="style.css"?>
            <message>Hello, styled XML!</message>
        ]]></example>
    </section>
    <section title="XML HttpRequest">
        <content>Introduces XMLHttpRequest for asynchronous data fetching in web applications.</content>
        <example><![CDATA[
            var xhttp = new XMLHttpRequest();
            xhttp.open("GET", "data.xml", true);
            xhttp.send();
        ]]></example>
    </section>
    <section title="XML Parser">
        <content>Explains XML parsing methods: DOM and SAX.</content>
        <example><![CDATA[
            let parser = new DOMParser();
            let xmlDoc = parser.parseFromString(xmlString, "text/xml");
        ]]></example>
    </section>
    <section title="XML DOM">
        <content>Details the Document Object Model (DOM) for accessing and modifying XML documents.</content>
        <example><![CDATA[
            let title = xmlDoc.getElementsByTagName("title")[0].childNodes[0].nodeValue;
        ]]></example>
    </section>
    <section title="XML XPath">
        <content>Describes XPath for navigating and querying XML documents.</content>
        <example><![CDATA[
            let nodes = xmlDoc.evaluate("//book/title", xmlDoc, null, XPathResult.ANY_TYPE, null);
        ]]></example>
    </section>
    <section title="XML XSLT">
        <content>Explains XSLT (Extensible Stylesheet Language Transformations) for XML formatting.</content>
        <example><![CDATA[
            <xsl:template match="/">
                <html>
                    <body>
                        <h2>Book List</h2>
                    </body>
                </html>
            </xsl:template>
        ]]></example>
    </section>
    <section title="XML XQuery">
        <content>Discusses XQuery for querying and manipulating XML data.</content>
        <example><![CDATA[
            for $x in doc("books.xml")/bookstore/book
            return $x/title
        ]]></example>
    </section>
    <section title="XML XLink">
        <content>Introduces XLink for creating hyperlinks in XML documents.</content>
        <example><![CDATA[
            <book xlink:href="http://example.com/book.xml"/>
        ]]></example>
    </section>
    <section title="XML Validator">
        <content>Explains how to validate XML documents for correctness.</content>
        <example><![CDATA[
            <note xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                  xsi:noNamespaceSchemaLocation="note.xsd">
                <to>Tove</to>
            </note>
        ]]></example>
    </section>
    <section title="XML DTD">
        <content>Describes Document Type Definition (DTD) for defining XML document structure.</content>
        <example><![CDATA[
            <!DOCTYPE note [
                <!ELEMENT note (to, from, message)>
            ]>
        ]]></example>
    </section>
    <section title="XML Schema">
        <content>Explains XML Schema (XSD) for defining XML document rules and constraints.</content>
        <example><![CDATA[
            <xs:element name="person">
                <xs:complexType>
                    <xs:sequence>
                        <xs:element name="name" type="xs:string"/>
                    </xs:sequence>
                </xs:complexType>
            </xs:element>
        ]]></example>
    </section>
    <section title="XML Server">
        <content>Discusses how XML is used in server-side applications.</content>
        <example><![CDATA[
            <response>
                <status>200</status>
                <message>Success</message>
            </response>
        ]]></example>
    </section>
</xml_tutorial>

