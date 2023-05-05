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
- รันคำสั่ง <code>apt upgrade</code> แล้วให้ตอบ <code>Y</code> ทุกอัน
