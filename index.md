*This documentation will eventually get updated*

## Features

* Test your vocabulary skills
* Import your own word lists
* Deploy it on your own server and curate your own lists and categorys (Language levels or classes)

## How to use

You can either test the app at [vocabulary.foxat.de](http://vocabulary.foxat.de/) or download the source code and deploy it on your own server. You will need PHP in order to run it on your own server.

## Tutorial: Create your own word list

Just create a .cvs file with the following structure:

Mother Language  | Foreign Language
---------------- | ----------------
word 1           | word 1 translation
word 2           | word 2 translation
...              | ...

The lanuguages in the header cells should be represented as their Countrys ISO Code. (Example: Germany - de, Italian - it)

## Tutorial: Curate your own public vocabulary lists

Inside the `/lists` directory, you can find the `lists.json` configuration File. The basic structure should look like this:

    [
        {
            name: 'List No. 1',
            languages: ['en', 'es'],
            category: 'Spanish Level 1',
            file: 'es-l1-no1.csv'
        },
        {
            name: 'Business Language',
            languages: ['de', 'en'],
            category: 'Englisch Klasse 10',
            file: 'business-10a.csv'
        }
    ]
    
To insert your own lists, make sure that you put in consistent categorys and language codes.
