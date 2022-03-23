# The OSI-Model

Cheat-Sheet for me, but if it can help you...

## Definition

When you start to learn how the **Network** works, you gonna see often the Model OSI (short for ``Open Systems Interconnection``). It was the first standard model for network communications

It was created in *1984* by the [ISO](https://www.iso.org/fr/home.html). This Model is really important for the communication between systems.

## How it is work ?

The OSI Model use **7 layers** :

-  7:    [Application](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Application)
-  6:    [Presentation](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Presentation)
-  5:    [Session](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Session)
-  4:    [Transport](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Transport)
-  3:    [Network](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Network)
-  2:    [Data Link](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Data-Link)
-  1:    [Physical](https://github.com/Vssksj/My_projects/blob/main/Cheat-Sheet/Network/OSI-Model.md#Physical)


And which one is important, you can't jump over a layer. For example, you can't go from *Data Link* to *Presentation*. Moreover, the layers can be cut in three parts:

  - **Software Layers** (7,6,5)
  - **Heart of OSI** (4)
  - **Hardware Layers** (3,2,1)


## Explantion

Now, there is short explanations of each **Layer**, *from 7 (Application) to 1 (Physical).*

### Application

It is the **Human-Computer** interaction, and we have protocols as *HTTP, FTP, DNS, ...*

### Presentation

This layer is used to *prepare* the data between two devices (encode, encrypt, ...).


### Session

Session layer is important when a device **talk** to an other device, because it **recognize and keep** the connection between the two devices.

### Transport

Transport layer is used to check if data is correctly and send fragments of data. It is the **Transport**.

### Network

There are two functions :

 - **Break and Rassembling** network packets
 - Try to find the **best path**

### Data Link

This layer establishes and terminates connections. Here, there are the **MAC Adress** and **Logical Link Control** (LLC).

### Physical

It is the physical materials 


## Conclusion

The *OSI-Model* is really useful for everybody !

*Note : It is a really short Cheat-Sheet for beginners*

### Source 

[Imperva](https://imperva.com/learn/application-security/osi-model/)
