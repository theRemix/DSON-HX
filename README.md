DSON-HX
=======

## Doge Serialized Object Notation for Haxe  
[http://dogeon.org](http://dogeon.org)

### Usage
```
var dson:Dson = new Dson( 'such "foo" is "bar", "doge" is "shibe" wow' );
trace(dson.toString());

dson = Dson.parseJson('{"foo": ["bar", "baz", "fizzbuzz"]}');
var json:Json = dson.toJson();

dson = Dson.fromJson({"foo": {"shiba": "inu", "doge": true}});
var obj:Dynamic = dson.toAny();
trace(obj.foo.doge)

```


#### Haxe targets supported:
- ~~C++~~
- ~~C#~~
- ~~Flash~~
- ~~Java~~
- ~~JavaScript~~
- Neko
- ~~PHP~~
- ~~Tamarin~~
- ~~Unity3d~~

Some examples of the DSON syntax and their JSON counterparts:

| DSON                                                            | JSON                                           |
| ----------------------------------------------------------------| ---------------------------------------------- |
| ```such "foo" is "bar", "doge" is "shibe" wow ```               | ```{"foo": "bar", "doge": "shibe"}```          |
| ```such "foo" is such "shiba" is "inu", "doge" is yes wow wow```| ```{"foo": {"shiba": "inu", "doge": true}} ``` |
| ```such "foo" is so "bar" also "baz" and "fizzbuzz" many wow``` | ```{"foo": ["bar", "baz", "fizzbuzz"]} ```     |
| ```such "foo" is 42very3 wow```                                 | ```{"foo": 34e3} ```                           |

#### Why?
Could be used for config files, you probably don't want to use this for anything not fun.

DRmXNWKUpahcXw7hcxDmAyd6oD8cHwE3zm  
to the moon!
