![Image_1](https://github.com/user-attachments/assets/0662984f-5a15-4410-ab1b-d0cbf220f8ed)
# Introduction
Over the last couple of years, I've seen a lot of lithophane projects, so I thought it was finally time to make my own. It seems like a significantly better alternative to laser engraving images and some early testing indicated better imaging quality with similar times for engraving/3D printing. I decided to create a lithophane of my amazing cat, Juno, in her halloween costume.
# Lithophane
To create the lithophane itself, I went to the following website: https://www.lithophanemaker.com/
 
I then scrolled down to "Flat Lithophane Maker." Here, I uploaded the file of my choosing, which was of my cat Juno in her halloween costume.
## Lithophane Specifications
I used the following settings:

Frame Options: Frame Only \
Crop: Yes \
Lithophane Resolution (mm/pixel): 0.2 \
Width (mm): 125 PLEASE KEEP THIS AT 125! \
Height (mm): 65 PLEASE KEEP THIS AT 65! \
Depth (mm): 7.5 \
Base Height (mm): 7.5 \
Overhang Angle (deg): 60 \
Maximum Thicknesss (mm): 3.0 \
Minimum Thickness (mm): 0.6 \
Stand Thickness (mm): 2 \
Stand Angle (degrees): 75

Once I had dialed these settings in, I clicked on "Create .stl." I extracted the file downloaded and 3D-printed it.
### Specifications & Material(s)
Below you can find the printer and material used.
#### 3D Printer
 Original Prusa Mini+
#### Material(s)
INLAND PLA 3D Printer Filament - 3D Printing PLA Filament 1.75mm, Dimensional Accuracy +/- 0.03mm - 1kg Cardboard Spool (2.2 lbs), Marble PLA
 – this can be purchased for $29.99 at the following link:
https://www.amazon.com/Inland-1-75mm-Marble-Printer-Filament/dp/B08M4733VV/ref=sr_1_3?crid=RY0788Z9D3XL&dib=eyJ2IjoiMSJ9.GvDUjGeacdaThMoKB2T31ewH9i3JmlLfhoDydChHBm-pD7cXPBEVjrKUewiIA1ZLE0_09V1n0PRn75b7hFqiDw4M0-lnl6NiRKwU4Bay_UQglrp8aVfnSITNRxxnTlk00zi7jk9JMRR5mzHilVguVNlu22jSBhxaIA2Mgu28qpM98QySMqZ0onKGj8rI2Ae99hyhSl7nTwlWuBccngRzfk5tlxoLLDb3Ck8adz-NTaQ.5vcyT03Wl1FkUx1DENvwhSOMvdqbl_TQCjXICAq7kSI&dib_tag=se&keywords=pla+filament+inland+marble&qid=1735843633&sprefix=pla+filament+inland+marble%2Caps%2C87&sr=8-3
#### Software
 PrusaSlicer
![Image_2](https://github.com/user-attachments/assets/a380fe96-3902-44ff-9e6b-a31b57fddf16)
#### Settings
  Layer Height: .2mm \
  Infill: 50% \
  Supports: Everywhere \
  Estimated Printing Time: 3 hour and 26 minutes - this will vary depending on your image

![Image_3](https://github.com/user-attachments/assets/f877f814-e1da-427f-9f4d-2340e025f6e6)

This project was created using EasyEDA, which is a PCB designing website. You can access it by going to: https://easyeda.com/

I highly recommend creating an account with Google, so it is easier to access later. After you have logged in, click on "Online Editor(Std Edition)." My current project looks like this:
![Image_2](https://github.com/user-attachments/assets/56d33924-dcb1-450c-96b9-7b57eb98293f)
When you open up the diagram, this is what you will see on my end:
![Image_3](https://github.com/user-attachments/assets/c1c175f7-895d-43a2-b9b8-416eb3fe3341)
Please note that, for some of these symbols, I went to user contributed symbols; to access these, go to Place then Symbol and search for the relevant symbol.

After I had created the circuit, I clicked on Design, then Convert Schematic to PCB. I moved around the components and clicked on Route and then Auto Route. I placed the NFC component on the back on purpose as well as the "Power" connection. The result is the following:
![Image_4](https://github.com/user-attachments/assets/fcf13c26-45eb-41a4-a2bf-af9358fd2908)
When I was ready to get my PCB created, I clicked on Fabrication then PCB Fabrication File (Gerber). You will get the following screen:
![Image_5](https://github.com/user-attachments/assets/84e913ee-8c45-444f-8f8b-cb427358a185)

Click on "Generate Gerber." This example is included in this project as well. You can then go to EasyEDA's partner website, https://jlcpcb.com/?href=easyeda-home, to order your PCB. Here, upload your .zip Gerber file and select additional customizations, like color. It usually ships within a few days and, hopefully, you will have your PCB in no time!

The next step is programming your NFC tag to include your specific details.
## NFC Tag
I have previously used these NFC tags for several projects, so I continue to rely on them.
![Image_4](https://github.com/user-attachments/assets/c1b4d1c5-4d13-4bfa-ba43-939e600c45c2)
The NFC tag is pretty simple to program using an Android phone and I’m sure you can use an iPhone as well.
# Initialization & Material(s)
Below you will find how I programmed the NFC tag and where it was purchased from.
## Initialization
I downloaded an app on the Play Store called NFC Tools; it is by wakdev. This app is incredibly useful and easy to use. When you first boot it up, this is what you’ll likely see:
![Image_5](https://github.com/user-attachments/assets/709e5967-18a4-4f82-8129-4af43c3fc6cd)
From here, tap your NFC tag; the following menu will appear.
![Image_6](https://github.com/user-attachments/assets/3fd644d4-7bb9-46e7-9eba-37c86f9be996)
Go to Write -> Add a record -> Contact. Enter your details.
![Image_7](https://github.com/user-attachments/assets/0435b498-c2f5-4c3b-ba01-dca678454fff)
The last thing left is the most critical: Make sure to press the “Write” button and then step away from your NFC tag and approach it again. Once it is completed, you should see this:
![Image_8](https://github.com/user-attachments/assets/204e200d-8ab7-4fe7-98e1-7b3b482a2dfd)
Now, the next time someone approaches this NFC, they will be prompted to add the contact.
## Material(s)
10pcs NFC Stickers Black NFC Tags NTAG215 NFC Sticker Tags 25MM Black NFC Stickers 504 Bytes Memory Programmable NFC Tags Compatible with Android iOS and NFC Enabled Phones Devices – this can be purchased for $7.96 at the following link:
https://www.amazon.com/Stickers-NTAG215-Programmable-Compatible-Android/dp/B091FCDPDR/ref=sxin_16_pa_sp_search_thematic_sspa?content-id=amzn1.sym.27b41115-b206-47c3-8621-713097e8442c%3Aamzn1.sym.27b41115-b206-47c3-8621-713097e8442c&crid=2CUK9W8I3L1WZ&cv_ct_cx=nfc%2Btags%2Bk%2Blakey&keywords=nfc%2Btags%2Bk%2Blakey&pd_rd_i=B091FCFJT9&pd_rd_r=1cfacf3c-cea7-49fc-9283-38dc8e35ebf4&pd_rd_w=3jGhz&pd_rd_wg=fOWr0&pf_rd_p=27b41115-b206-47c3-8621-713097e8442c&pf_rd_r=T2JE71K6VYQHEHNZ605T&qid=1735842929&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=nfc%2Btags%2Bk%2Blakey%2Caps%2C74&sr=1-1-6024b2a3-78e4-4fed-8fed-e1613be3bcce-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9zZWFyY2hfdGhlbWF0aWM&th=1
# Tips
You might want to get the surface-mounted components to fully complete this PCB, but it is not necessary. If you do, however, I recommend using a heat gun to help out with soldering the connections since it can be a bit tricky.

You may have an issue ensuring that your phone can read the NFC tag. I recommend, for at least Android and the process is likely similar for iOS, going to Settings -> Connected Devices -> Connection Preferences -> NFC (and turn this on).

People trying to read the NFC tag may also have issues if their phone has a thick case or if they are not tapping the correct part of the phone to the NFC tag. Removing the case and moving the phone around until it reads the tag helps with this, but this is easier for some than others.
