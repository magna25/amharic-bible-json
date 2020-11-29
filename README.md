# amharic-bible-json

A JSON representation of the entire amharic bible as a single json file and also a collection of individual books.

The conversion was done by downloading and parsing the html version of the bible from the https://www.wordproject.org/bibles/am/. Some missing data was filled manually from http://bible.geezexperience.com/amharic/


I haven't checked each book or verses for consistency so there might be a chance that some data might be missing but overall it's a complete copy.


## Notes ##

Unlike the KJV or NASB translation, the amharic translation occasionaly combines two verses in to one and those are denoted on hardcover as start-end. 


Ex. Genesis 7:2-3

    2 You shall take [a]with you [b]seven pairs of every clean animal, a male and his female; and two of the animals that are not clean, a male and his female; 3 also of the birds of the sky, seven pairs, male and female, to keep their offspring alive on the face of all the earth.


But on the Amharic version verse 2 and 3 don't exist individually and are denoted like the below on a hardcover.

     2-3 ከንጹሕ እንስሳ ሁሉ ሰባት ሰባት ተባትና እንስት፥ ንጹሕ ካልሆነ እንስሳም ሁለት ሁለት ተባትና እንስት፥ ከሰማይ ወፍ ደግሞ ሰባት ሰባት ተባትና እንስት እያደረግህ በምድር ላይ ለዘር ይቀር ዘንድ ለአንተ ትወስዳለህ።


In the JSON files, this is denoted by ommitting the text from the first verse and instead storing it on the last one. In the above example Genesis 7:2 would return an empty text. If you want to Genesis 7:2, you would have to look for Genesis 7:3 instead.


<br/>
<br/>
You are free to use this data for any project.