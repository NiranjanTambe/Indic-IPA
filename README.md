# Indic-IPA
X11 keyboards allow us to modify the existing mapping &amp; form new keyboards. This is an attempt to form a keyboard based on very popular inscript layout. This keyboard can roughly be useful for transcribing major Indo-Aryan languages. eg. Marathi, Hindi, Urdu, Gujarati, Bangla, Konkani, Kashmiri. Documentation has all the instructions about how to add a new character or replace an existing character.

# How to install
This keyboard is very easy to install. You have to follow 3 steps.

- Add the keyboard code file (IIPA) to the following path -

```
/usr/share/X11/xkb/symbols/
```

- Replace the `evdev.xml` file present in the following path with the file uploaded provided in this repository.
```
/usr/share/X11/xkb/rules/
```

OR

Paste this code exactly after the end of one layout. A layout starts with `<layout>` and ends with the same. In between these two lies the description of a particular keyboard required by the system.

```
<layout>
  <configItem>
      <name>IIPA</name>
      <shortDescription>IIPA</shortDescription>
      <description>Indic IPA</description>
    <languageList><iso639Id>eng</iso639Id></languageList>
  </configItem>
<variantList/>
</layout>    
```

That's it! You are ready to use a customized IPA keyboard.

# Acknowledgement

This work is possible because of the instructions found on [this](http://people.uleth.ca/~daniel.odonnell/Blog/custom-keyboard-in-linuxx11) blog maintained by Mr. Danel Paul O'Donnell. I am deeply indebted to him for this explanation. I would also like to thank Mr. Sushant Devalekar for motivating me to upload this code as a licensed github repository.
