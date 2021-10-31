# Add your Java Programs here:

## 1. Program to Check Whether a Number is Prime or Not:
```
public class Main {

  public static void main(String[] args) {

    int num = 29;
    boolean flag = false;
    for (int i = 2; i <= num / 2; ++i) {
      // condition for nonprime number
      if (num % i == 0) {
        flag = true;
        break;
      }
    }

    if (!flag)
      System.out.println(num + " is a prime number.");
    else
      System.out.println(num + " is not a prime number.");
  }
}
```
### Output:
```
29 is a prime number.
```

## 2. Program to Check Prime Number using a while loop:
```
public class Main {

  public static void main(String[] args) {

    int num = 33, i = 2;
    boolean flag = false;
    while (i <= num / 2) {
      // condition for nonprime number
      if (num % i == 0) {
        flag = true;
        break;
      }

      ++i;
    }

    if (!flag)
      System.out.println(num + " is a prime number.");
    else
      System.out.println(num + " is not a prime number.");
  }
}
```
### Output:
```
33 is not a prime number.
```

## 3. Program to Check Leap Year:
```
public class Main {

  public static void main(String[] args) {

    // year to be checked
    int year = 1996;
    boolean leap = false;

    // if the year is divided by 4
    if (year % 4 == 0) {

      // if the year is century
      if (year % 100 == 0) {

        // if year is divided by 400
        // then it is a leap year
        if (year % 400 == 0)
          leap = true;
        else
          leap = false;
      }
      
      // if the year is not century
      else
        leap = true;
    }
    
    else
      leap = false;

    if (leap)
      System.out.println(year + " is a leap year.");
    else
      System.out.println(year + " is not a leap year.");
  }
}
```
### Output:
```
1900 is not a leap year.
```

## 4. Program to Lookup enum by String value:
```
public class EnumString {

    public enum TextStyle {
        BOLD, ITALICS, UNDERLINE, STRIKETHROUGH
    }

    public static void main(String[] args) {

        String style = "Bold";

        TextStyle textStyle = TextStyle.valueOf(style.toUpperCase());

        System.out.println(textStyle);
    }
}
```
### Output:
```
BOLD
```
