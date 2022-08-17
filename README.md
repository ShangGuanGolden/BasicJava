# Java-infomation-example-code-

import java.util.HashMap;
public class L2Unit1Mission5HashMaps {

	public static void main(String[] args) {

		HashMap<String,Integer> list = new HashMap<String,Integer>();//first parameter is the key and the second is the value		
		list.put("One", 1); //adds a value 
		System.out.println(list.put("One", 1)); // prints 1
		
		System.out.println(list.put("Two", 2)); //prints null because we added a new key and value
		
		System.out.println(list.get("Two")); //prints the value of Two
		
		System.out.println(list.getOrDefault("Zero", -123456)); // prints out the value zero assigned or -123456 if there isn't one
	
        list.replace("Two", 4);
        
        System.out.println(list.get("Two"));
        
        System.out.println(list.replace("Two",2));
        System.out.println(list.get("Two"));
        System.out.println(list.replace("Zero", 0));
        
        list.remove("Two"); // removes the key two and its value
        list.remove("One", 2); //it won't remove the value because 2 didn't exist in the beginning
        
        System.out.println(list.size()); //prints the size
        System.out.println(list.isEmpty()); //checks if the list is empty or not
        System.out.println(list.keySet()); //give the name of the keys
        System.out.println(list.values()); //gives the value stored in the keys.
        System.out.println(list.containsKey("Two")); //checks if the key "Two" exists or not
        System.out.println(list.containsValue("1")); //checks if the value "1" exists or not
        
        
        
        
        
	}

}
