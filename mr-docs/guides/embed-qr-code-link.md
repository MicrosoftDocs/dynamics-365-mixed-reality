

# Embed a link in a QR code to make it easy to open a guide in Dynamics 365 Guides

A Microsoft Dynamics 365 Guides author can embed a link to a guide in a QR code to make it easy for operators to open the guide on Microsoft HoloLens. The link can open a guide or 
go to a specific step within a guide.

An operator can access the QR code in two different ways:

- **Printed QR code**. Operators can use a printed QR code to open a guide and anchor the holographic content at the same time. This makes it easy for operators to 
launch a guide quickly by gazing at a contextual printed QR code attached to the area where they need to do their work, and anchor their holographic content 
to the same QR code.

- **Digital QR code**. Operators can use a digital QR code to open a guide without anchoring the guide. In this case, authors must provide another 
anchoring method for operators to align their holograms. Using a digital QR code is useful if you want to assign a guide to digital work instructions, 
or if you need a quick way for an operator to launch a guide when they don't have access to a printed QR code.

## Embed a link in a QR code

1. [Create a guide link](pc-app-copy-link-guide-step.md). 

2. Use a third-party QR code generator to create a QR code. Microsoft recommends the following third-party QR code generators:

    - [http://goqr.me/](http://goqr.me/)    
    
    - [https://www.qr-code-generator.com/](https://www.qr-code-generator.com/)
    
    - [https://www.the-qrcode-generator.com/](https://www.the-qrcode-generator.com/)

 
    > [!NOTE]
    > When you use any third-party QR code generator, the QR code generator receives access to the string of your guides link.
    
3. Copy the link from step 1, paste it into the QR code.

4. Download the QR code.

5. Do one of the following:

    - Add the digital QR code to a digital document for an operator to use.
    
    - Print the QR code and attach it to a physical part in the real-world environment where the work takes place.
    
    > [!IMPORANT]
    > When creating a printed QR code with an embedded link, make sure to follow [best practices for QR codes](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors).
