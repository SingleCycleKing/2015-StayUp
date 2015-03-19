#2015 Unique Studio Android Team Stay Up Examination (Part B)


#####Tip: If you are freshman, please finish the questions of part B. If you choose to finish the questions of part A, however, you can gain double scores. If you are sophomore, you must finish the questions of part A.


## Multiple Choice Question (10 Points)

- Which one of these lists contains only Java programming language keywords？<br/>
A.class, if, void, long, Int, continue <br/>
B.goto, instanceof, native, finally, default, throws <br/>
C.try, virtual, throw, final, volatile, transient <br/>
D.strictfp, constant, super, implements, do <br/>

- What is the data type of the number 10.1?<br/>
A.float<br/>
B.double<br/>
C.unsigned float<br/>
D.class<br/>

- All wrapper classes such as Interger,Boolean and Double in JAVA are<br/>
A.are protected<br/>
B.are private<br/>
C.are final<br/>
D.are serializable<br/>

- Multiple inheritance means <br/>
A.one class inheriting from more super classes<br/>
B.more classes inheriting from one super class<br/>
C.more classes inheriting from more super classes<br/>
D.None of the above<br/>

- Which of the following is true?<br/>
A.finally block is executed before the catch block but after the try block.<br/>
B.A finally block is executed, only after the catch block is executed.<br/>
C.A finally block is executed whether an exception is thrown or not.<br/>
D.A finally block is executed, only if an exception occurs.<br/>

##Subjective Item

###1.JAVA Basic Question (15 Points)
- Please consider the follow codes and tell us what will be output.
Tip: Please pay attention to the order of the output.

```java

class Unique {
  public Unique() {
    System.out.println("Hello Unique");
  }

  {
    System.out.println("I'm in Unique");
  }

  static {
    System.out.println("static unique");
  }
}

public class Android extends Unique {
  public Android() {
    System.out.println("Hello Android");
  }

  {
    System.out.println("I'm in Android");
  }

  static {
    System.out.println("static android");
  }

  public static void main(String[] args) {
    new Unique();
    new Android();
  }
}

```

###2.Algorithm (15Points)
```java
//TODO
```

###3.Http (15 Points)

- Please write down the HTTP request that the server socket will receive according to the client code below:

```java

URL url = new URL("http://hustunique.com:80/exgfs.json?from=1449803471000");

HttpURLConnection conn = (HttpURLConnection) url.openConnection();

conn.setRequestMethod("POST");
conn.setDoOutput(true);

conn.setRequestProperty("User-Agent", "UniqueStudio Spider");

String data = "username=NIANTIC&password=Sk9JTiBUSEUgUkVTSVNUQU5DRSBJVCBJUyBUSU1FIFRPIE1PVkU"

OutputStream out = conn.getOutputStream();
out.write(data.getBytes());
out.flush();
out.close();

int responseCode = conn.connect();
```

###4.Database (20 Points)
- Structured Query Language (SQL) is a coding language which is used to design dababase. It is usually used to access to database. Thus we ask you to learn how to use it. For android developer, google has developed a helper which is called as SQLiteOpemHelper. Please try to have access to a database and insert a data into database whit helper. Here are some keywords for you: ContentValues and SQLiteDatabase.<br>
Tip:[SQLiteDatabase](http://developer.android.com/reference/android/database/sqlite/SQLiteDatabase.html) [SQLiteOpenHelper](http://developer.android.com/reference/android/database/sqlite/SQLiteOpenHelper.html) [ContentValues](http://developer.android.com/reference/android/content/ContentValues.html)

- SQLiteDatabase can also execute your own sql sentences. Please try to create a table named user with execSQL. And the first column of the table is named userid(int). The second of that is named username(character string).

- The number of columns is not increased with the following sentence. Please tell me why.
```java
db.execSQL("INSERT INTO user ('201','kami_control','godness')");
```

###5.Android (25 Points)

- Try to complete a simple app. There are two interfaces like the following pictures in the app. [Here are some tips](http://developer.android.com/guide/topics/ui/controls.html)
 ![](https://github.com/SingleCycleKing/UniqueStudio/blob/master/img/1.png)
 ![](https://github.com/SingleCycleKing/UniqueStudio/blob/master/img/2.png)


- Show the basic data at the second page which is filled at the first page.  

- When user click "select avatar" or "select background", it will open gallery. Please show the pictures at the second page if you can. [Tips Here](http://stackoverflow.com/questions/11144783/how-to-access-an-image-from-the-phones-photo-gallery)
