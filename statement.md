```java runnable
// { autofold
import java.util.Map;
import java.util.HashMap;

public class Main {

public static void main(String[] args) {
// }
Map<String, String> map = new HashMap<String, String>();
map.put("first_name", "Alvin");
map.put("last_name",  "Alexander");

// java 8
map.forEach((k,v)->System.out.println("key: " + k + ", value: " + v));
// { autofold 
}

}
//}
```

```java runnable
import java.util.HashMap;
import java.util.Map;

public class Main {
    
    public static void main(String[] args) {
        
        Map<String, String> map = new HashMap<String, String>();
        map.put("first_name", "Alvin");
        map.put("last_name",  "Alexander");

        // java 8
        map.forEach((k,v)->System.out.println("key: " + k + ", value: " + v));

        // prior to java 8
        for (Map.Entry<String, String> entry : map.entrySet()) {
            System.out.println("key: " + entry.getKey() + ", value: " + entry.getValue());
        }

    }

}
```
