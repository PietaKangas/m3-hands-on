### Part A: 
ghost text: 
    // Add fields here                    
    // Add static mapper here
    // Add any other methods here


ghost text after opening User.java: 
    // Add fields here
    // Add static fromUser(User) mapper here
    // Add any other methods here

The code text changed a little bit. 

### Part B:

Ai's text: 
public static UserDTO fromUser(User user) {
        return new UserDTO(user.getId(), user.getName(), user.getEmail(), user.isActive());
    } 

- Was good enough, so i didnt change anything

- added main:
 public class Main {
    public static void main(String[] args) {
        User user = new User(123456, "Lisa", "lisa@example.com", true);
        
        UserDTO dto = UserDTO.fromUser(user);
        
        System.out.println(dto);
    }
}

Print: UserDTO[id=123456, name=Lisa, email=lisa@example.com, active=true]


### Part C:

Read the ghost text before accepting. Are the annotations, response types, and status
codes consistent with the hand-written endpoint?

Added GetMapping and PostMapping annotations

- Now annotation lines are only there where I added (or AI) them, listOrders doesn't have it.
- The file style is not fully consistent
- The Javadoc above the class refers to createOrder(String, int), but the AI ​​wrote the method as createOrder(@RequestBody Order order) so the tests don't compile. 
-


