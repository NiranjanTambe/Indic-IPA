# Indic-IPA
This is an attempt to form an IPA keyboard based on the very popular Inscript layout for Indian languages. This keyboard can roughly be useful for transcribing major Indo-Aryan languages. eg. Marathi, Hindi, Urdu, Gujarati, Bangla, Konkani, Kashmiri. Following are the instructions for the installation.

# How to install
- Add the keyboard code file (IIPA) to the following path -

```
/X11/xkb/symbols/
```
One first has to locate this path on their system.

- Paste this code exactly after the end of one layout. (A layout starts with `<layout>` and ends with </layout>.)

```
<layout>
<configItem>
	<name>IIPA</name>
	<shortDescription>IIPA</shortDescription>
	<description>Indic IPA</description>
	<languageList><iso639Id>eng</iso639Id></languageList>
</configItem>
</layout>    
```

That's it! You are ready to use a customized IPA keyboard made especially for Indian languages.

# Acknowledgement
This work is possible because of the instructions found on [this](http://people.uleth.ca/~daniel.odonnell/Blog/custom-keyboard-in-linuxx11) blog maintained by Mr. Danel Paul O'Donnell. I am deeply indebted to him for this explanation. I would also like to thank Mr. Sushant Devalekar for motivating me to upload this code as a github repository.
