+++
author = "Denver Noell"
date = 2019-03-05T00:00:00Z
description = "How to use Steel Helper sites"
tags = ["Steel", "Civil Engineering"]
title = "Steel Helper"
[[images]]
  src = "static/img/2019/03/pic02.jpg"
  alt = "Desert Scene"
  stretch = "stretchH"
+++
Starting my Steel class, I could tell immediately that the problems in this class had lots of opportunity to be programmed due to the reliance on code. This means that any cutting back on referring to the code book can be very beneficial.

This was dope because...

Emoji can be enabled in a Hugo project in a number of ways.
<!--more-->
The [`emojify`](https://gohugo.io/functions/emojify/) function can be called directly in templates or [Inline Shortcodes](https://gohugo.io/templates/shortcode-templates/#inline-shortcodes).

To enable emoji globally, set `enableEmoji` to `true` in your site’s [configuration](https://gohugo.io/getting-started/configuration/) and then you can type emoji shorthand codes directly in content files; e.g.

<p><span class="nowrap"><span class="emojify">🙈</span> <code>:see_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙉</span> <code>:hear_no_evil:</code></span>  <span class="nowrap"><span class="emojify">🙊</span> <code>:speak_no_evil:</code></span></p>
<br>

The [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/) is a useful reference for emoji shorthand codes.

***

**N.B.** The above steps enable Unicode Standard emoji characters and sequences in Hugo, however the rendering of these glyphs depends on the browser and the platform. To style the emoji you can either use a third party emoji font or a font stack; e.g.

{{< highlight html >}}
.emoji {
font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
}
{{< /highlight >}}

{{< css.inline >}}
<style>
.emojify {
font-family: Apple Color Emoji,Segoe UI Emoji,NotoColorEmoji,Segoe UI Symbol,Android Emoji,EmojiSymbols;
font-size: 2rem;
vertical-align: middle;
}
@media screen and (max-width:650px) {
.nowrap {
display: block;
margin: 25px 0;
}
}
</style>
{{< /css.inline >}}