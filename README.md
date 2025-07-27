# SH1106 Update

- Remove redundant scroll as SH1106 doesn't implement this in software
- Add scroll function in software (WIP - Thinking in progress)
- Copyright belongs to Adafruit
- Not production ready - Using this to learn uc coding as way to get over mental fatigue
- Will be committing everything to main branch as the guy behind this is lazy 

## Notes 
- I am using a 38 PIN ESP32 For testing the scketches and in my case I got the SH1106 OLED to work using the following SDA and SCL/SCK configurations. 
```c
#define OLED_SDA 27
#define OLED_SCL 26
```

- As I learn more, I will try with other pin combinations to see if still works.
- This experimentation will come after implementing software scroll (hope to do it without breaking the signature)

## Personal Todo List
1. Implement A hacky software scroll
2. Refactor the hacky scroll so that this becomes a drop in replacment for previous versions of Adafruit_SH1106 forks
3. Update the code to work with RP2040 / RP2350
