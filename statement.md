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
//{ autofold
}

}
//}
```
