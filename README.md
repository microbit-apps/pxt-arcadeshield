# MakeCode extension: Arcade Shield for BBC micro:bit (V2)

This MakeCode extension allows you to use any of the  MakeCode Arcade shields with the MakeCode for BBC micro:bit editor. The extension provides access 
to the screen and buttons on the shield, and has
a Bitmap abstraction with numerous drawing primitives
(draw line, circle, square, etc).
Bitmaps also can be created using the built-in
image editor in MakeCode.

> **NOTE: This extension will only work in https://makecode.microbit.org/beta**. The extension is still under development and is subject to changes. Please file issues at https://github.com/microbit-apps/pxt-arcadeshield/issues 

## Arcade Shields for the micro:bit V2

Various Arcade shields for the micro:bit V2 are available on the market today, including:

<table>
<tr valign="top">
<td width="33%" >
<a href="https://www.kittenbot.cc/products/newbit-arcade-shield">
Kittenbot's newbit Arcade shield
</a>
</td><td width="33%" >
<a href="https://shop.elecfreaks.com/products/micro-bit-retro-programming-arcade">
ELECFREAK's micro:bit Arcade shield
</a>
</td>
<td width="33%" >
<a href="https://www.icshop.com.tw/products/368112100137?locale=en">
ICShopping's Game:bit Arcade shield
</a>
</td></tr>
<tr>
<td>
<a alt="Kittenbot's newbit Arcade shield" href="https://www.kittenbot.cc/products/newbit-arcade-shield">
<img src="assets/newbit-shield.png">
</a>
</td><td>
<a alt="ELECFREAK's micro:bit Retro Arcade shield" href="https://shop.elecfreaks.com/products/micro-bit-retro-programming-arcade">
<img src="assets/elecfreaks-shield.png">
</a>
</td><td>
<a alt="ICShopping's Game:bit" href="https://www.icshop.com.tw/products/368112100137?locale=en">
<img src="assets/gamebit-shield.png">
</a>
</td></tr>
<tr valign="top">
<td>

Small screen. No battery or battery pack included. 3.7V JST power jack on back. One <a href="https://aka.ms/jacdac">Jacdac</a> port.

</td>

<td>

Assembly required. Small screen. AAA Battery pack on back. One <a href="https://aka.ms/jacdac">Jacdac</a> port.

</td>
<td>

No assembly required. Large screen and 3d-printed enclosure with LiPo battery inside. Two <a href="https://aka.ms/jacdac">Jacdac</a> ports.

</td>
</tr>

</table>


## Simulator support

As shown below, the extension provides a simulator for the display,
with keyboard controls mapping to the inputs of
the display shield (A and B buttons, and the four directions of the
D-pad, see arrow buttons).  Blocks
for the shield are under the toolbox categories `Controller` and
`Drawing` and are described further below.

![MakeCode with Arcade Shield Simulator](./assets/shieldSim.png)

## Blocks

The examples below are illustrative. All blocks have their own
detailed help pages, available from the MakeCode editor. 
More APIs are available via TypeScript.

### Controller

The controller API has event handlers for the A,B and four directions
on the D-pad, as well as the menu button. There also are functions
for polling the buttons. Some example code:

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    screen().fill(Math.randomRange(1,14))
})
controller.left.onEvent(ControllerButtonEvent.Pressed, function () {
    screen().fill(15)
})
```

Display present/absent
```blocks
```

### Drawing with bitmaps

## TypeScript APIs

# Supported targets

- for PXT/microbit

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script
