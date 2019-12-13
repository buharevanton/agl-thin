In order to make button "Register and Create Room" work for **Poker** project - 
place `@CrossOrigin("*")` annotation at:
```
public class RoomController {
...
    @CrossOrigin("*")
    @PostMapping(path = "/room", consumes = MediaType.APPLICATION_JSON_UTF8_VALUE)
    public ResponseEntity<Room> createRoom(@RequestBody Room roomToRegister) {


public class TemporaryRegistrationController {
...
    @CrossOrigin("*")
    @PostMapping(path = "/temporary-registration", consumes = MediaType.APPLICATION_JSON_UTF8_VALUE)
    public ResponseEntity registerTemporaryUser(@RequestBody @Valid TemporaryUser temporaryUser) {

```  

