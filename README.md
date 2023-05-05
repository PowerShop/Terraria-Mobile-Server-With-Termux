# Terraria Mobile Server With Termux

I'm trying to open a mobile terraria server with Termux and Host by <a href="serveo.net">serveo.net</a>

## First you need to install Termux (<a href="https://play.google.com/store/apps/details?id=com.termux&hl=th&gl=US">Here</a>)

<img src="https://i.imgur.com/He8a0X2.png">
<hr>
- หลังจากติดตั้งแล้วให้เปิด Termux ขึ้นมา
- รันคำสั่ง <code>termux-change-repo</code> เพื่อเปลี่ยน Mirror repo ของ termux
- หลังจากรันแล้วจะมีหน้าต่างปรากฏขึ้นมาดังภาพ ให้เอานิ้วจิ้มที่ <code>OK</code> หรือจะกด <code>Enter</code> บนแป้นพิมพ์มือถือก็ได้
<img src="https://i.imgur.com/xmLradd.png">
<hr>
- เมื่อกด <code>OK</code> จะปรากฎอีกหน้าต่างขึ้นมาดังภาพ ให้เอานิ้วจิ้มเลือกที่ <code>Mirror by BFSU></code> แล้วจิ้มที่ <code>OK</code>
<img src="https://i.imgur.com/Awcz4ay.png">
<hr>
- รันคำสั่ง <code>apt install openssh</code> แล้ว Console จะถามว่า <code>Do you want to continue? (Y/n)</code> ให้ตอบ <code>Y</code> แล้ว Enter
<img src="https://i.imgur.com/J5GZnWA.png">
<hr>
- รันคำสั่ง <code>apt upgrade</code> แล้วให้ตอบ <code>Y</code> ทุกอัน <br>
- หลังจาก Upgrade เสร็จแล้ว ให้รันคำสั่ง <code>ssh -R โดนเมนของเรา:7777:localhost:7777 serveo.net</code> แล้ว <code>Enter</code> <br>
- โดเมนของเรา = ตั้งอะไรก็ได้ สั้นหรือยาวก็ได้ เช่น <code>ssh -R jothan:7777:localhost:7777 serveo.net</code> <br>
- หลังจากรันคำสั่งไปแล้วจะขึ้นหน้าต่างดังภาพ ให้ตอบ <code>yes</code> แล้ว <code>Enter</code> <br>
<img src="https://i.imgur.com/mcro3rT.png">
<hr>
- หากขึ้นว่า <font color="green">Forwarding TCP conections from serveo.net:7777</font> ถือว่าเชื่อมต่อสำเร็จ <br>
- ต่อไปให้เข้าเกม Terraria ในมือถือของเรา แล้วเปิดเซิร์ฟเวอร์ด้วยการ Host จากเครื่องเรา และเวลาจะให้เพื่อนเชื่อมต่อ ให้ใช้ IP : <code>โดเมนที่เราตั้ง.serveo.net</code> Port : <code>7777</code>
<br>

# English README
# Terraria Mobile Server with Termux

This guide will help you set up a Terraria mobile server using Termux and host it with [Serveo.net](https://serveo.net/).

## Prerequisites

Before starting, make sure you have [Termux](https://play.google.com/store/apps/details?id=com.termux&hl=th&gl=US) installed on your device.

## Changing Termux repository mirror

1. Open Termux.
2. Run the command `termux-change-repo` to change the mirror repository of Termux.
3. A window will appear. Tap on `OK` or press `Enter` on your mobile keyboard.
4. Another window will appear. Select `Mirror by BFSU>` by tapping on it and then tap on `OK`.

## Installing and upgrading packages

1. Run the command `apt install openssh` to install the OpenSSH package. When prompted with `(Y/n)`, enter `Y` and press `Enter`.
2. Run the command `apt upgrade` to upgrade all packages. When prompted with `(Y/n)`, enter `Y` and press `Enter`.

## Hosting the server with Serveo.net

1. Run the command `ssh -R <yourdomain>:7777:localhost:7777 serveo.net` to host the server with Serveo.net. Replace `<yourdomain>` with a domain name of your choice. For example, `ssh -R jothan:7777:localhost:7777 serveo.net`.
2. When prompted with a message about the authenticity of the host, enter `yes` and press `Enter`.
3. If you see `Forwarding TCP connections from serveo.net:7777`, the connection is successful.

## Connecting to the server

1. Open Terraria on your mobile device and host a server using your device.
2. To allow your friends to join, give them the IP address `<yourdomain>.serveo.net` and the port `7777`.

**Note:** The server will only be available as long as Termux is running. To stop the server, close the Termux app.
