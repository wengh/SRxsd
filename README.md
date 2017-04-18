# SRxsd
XSD schemas for SimpleRockets XML files

To get IntelliSense feature in Visual Studio:
1. Move `SR` folder and it's contents to `<Visual Studio Path>/Xml/Schemas/`
2. Insert these codes into `catalog.xml`
    ```xml
    <Schema targetNamespace="http://jundroo.com/simplerockets/partlist.xsd" href="%InstallRoot%/xml/schemas/SR/partlist.xsd"/>
    <Schema targetNamespace="http://jundroo.com/simplerockets/solarsystem.xsd" href="%InstallRoot%/xml/schemas/SR/solarsystem.xsd"/>
    <Schema targetNamespace="SRTextureAtlas" href="%InstallRoot%/xml/schemas/SR/textureatlas.xsd"/>
    <Schema targetNamespace="SRShip" href="%InstallRoot%/xml/schemas/SR/ship.xsd"/>
    ```
3. Add:
    + `xmlns="http://jundroo.com/simplerockets/partlist.xsd"` in `<PartTypes>`
    + `xmlns="http://jundroo.com/simplerockets/solarsystem.xsd"` in `<SolarSystem>`
    + `xmlns="SRTextureAtlas` in `<TextureAtlas>`
    + `xmlns="SRShip"` in `<Ship>`
