# githubactions
github actions


###### Class 1
<table align="center">
  
  <tr>
  <th>Class Before</th>
  <th>Class After</th>
  </tr>
  
  <tr> 
  <td>
  
  ```java
public class Main {
    public static void main(String args[]){

        Duck d1 = new SoDuck();
        d1.swim();
        d1.perform();

        Duck d2 = new YellowDuck();
        d2.swim();
        d2.perform();

        ((SoDuck)d1).gotShot();
        d1.perform();
    }
}
```
  
  
  </td>
  
  <td>


```java

public class SoDuck extends Duck{

    @Override
    protected String display() {
        return "Hey, I am SoDuck";
    }
    public SoDuck(){
        super();
        this.myFlyBehaviour = new FlyWithWings();
    }
    public void gotShot(){
        System.out.println("Got shot -> No Fly");
        this.myFlyBehaviour = new NoFly();
    }
}

```


</td>
</tr>
  </table>
