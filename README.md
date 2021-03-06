Voyage [![Build Status](https://travis-ci.org/pharo-nosql/voyage.png)](http://travis-ci.org/pharo-nosql/voyage) [![Test Status](https://api.bob-bench.org/v1/badgeByUrl?branch=master&hosting=github&ci=travis-ci&repo=pharo-nosql%2Fvoyage)](https://bob-bench.org/r/gh/pharo-nosql/voyage)
======


Voyage is an object persistence abstraction layer for Pharo.

Install
-------

Just install it from you Pharo catalog. 

You can also install it executing scripts:

### Voyage-Mongo
```Smalltalk
Metacello new 
	repository: 'github://pharo-nosql/voyage/mc';
	baseline: 'Voyage';
	load: 'mongo tests'.
```

### Voyage-UnQLite
```Smalltalk
Metacello new 
	repository: 'github://pharo-nosql/voyage/mc';
	baseline: 'Voyage';
	load: 'unqlite tests'.
```

### Installing in Pharo 3.0 and Pharo 4.0
We develop Voyage in latest Pharo version and keep backward compatibility with previous versions, which 
is usually ok but sometimes to gain something we lose something. 
Since some time, we use "metadataless"  filetree format, which is not present previous versions. 
To be able to install Voyage, before anything you need to install latest [metacello](https://github.com/dalehenrich/metacello-work):

```Smalltalk
Metacello new
  baseline: 'Metacello';
  repository: 'github://dalehenrich/metacello-work:master/repository';
  get.
Metacello new
  baseline: 'Metacello';
  repository: 'github://dalehenrich/metacello-work:master/repository';
  onConflict: [:ex | ex allow];
  load
```

Documentation
-------------
### Pharo for the enterprise book
Voyage is part of the upcoming "Pharo for the Enterprise 2" book, and Johan Fabry (along with Damien Cassou) has written a nice chapter on it: [HTML](https://ci.inria.fr/pharo-contribution/job/EnterprisePharoBook/lastSuccessfulBuild/artifact/book-result/Voyage/Voyage.html) / [PDF](https://ci.inria.fr/pharo-contribution/job/EnterprisePharoBook/lastSuccessfulBuild/artifact/book-result/Voyage/Voyage.pdf)

### Others
- http://smallworks.eu/web/blog/2013-06-14-voyage-the-adventure
- http://smallworks.eu/web/blog/2013-07-18-Voyage-advanced-queries
- [Voyage by example, talk at ESUG 2014](http://smallworks.eu/web/blog/2014-08-21-VoyageByExample)
