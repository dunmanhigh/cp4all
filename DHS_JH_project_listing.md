# Junior High Computing Projects

Use this place as (1) a portal to access others' projects, or (2) as a place to list your project for others to improve.

### (1) Improve others' projects

Instructions:
1. Scroll down and click on the links to people's repositories.
2. Test run their code by copying and pasting their code into something like http://create.withcode.uk/ .
3. In their GitHub repository, click on edit to suggest changes to their code. 
4. Submit your changes as a pull request.    

### (2) Add projects that would benefit our community!

To list your project below, click on edit, make your change (follow the markdown format: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#tables) then submit it as a pull request.


Note: Only VALID and NEW entries will be accepted.


The first row is done as an example for you.


| Project Title | Project Description (i.e. How is your project unique from others?) | Contribution needed | Link to GitHub repository | Student Name | Class |
| post-exam_bot | HI | contribution needed | https://github.com/FailureNoob/post-exam_bot/tree/main | Chloe Te Yu En | 2A |

print("Title of program: Post-exam bot")
print()
while True:
  description = input("Could you describe how you feel in a sentence?")

  list_of_words = description.split()

  feelings_list = []
  encouragement_list = []
  counter = 0
  
  for each_word in list_of_words:
    
    if each_word == "bored":
      feelings_list.append("bored")
      encouragement_list.append("find something fun to do")
      counter += 1
    if each_word == "enjoying":
      feelings_list.append("enjoying")
      encouragement_list.append("remember to share the fun with others")
      counter += 1
    if each_word == "results":
      feelings_list.append("results")
      encouragement_list.append("just do your best!")
      counter += 1
    if each_word == "sad":
      feelings_list.append("sad")
      encouragement_list.append("don't give up!")
      counter += 1

  if counter == 0:
    
      output = "Sorry I don't really understand. Please use different words?"

  elif counter == 1:
    
      output = "It seems that you are feeling quite " + feelings_list[0] + ". However, do remember that "+ encouragement_list[0] + "! Hope you feel better :)"  

  else:

    feelings = ""    
    for i in range(len(feelings_list)-1):
      feelings += feelings_list[i] + ", "
    feelings += "and " + feelings_list[-1]
    
    encouragement = ""    
    for j in range(len(encouragement_list)-1):
      encouragement += encouragement_list[i] + ", "
    encouragement += "and " + encouragement_list[-1]

    output = "It seems that you are feeling quite " + feelings + ". Please always remember "+ encouragement + "! Hope you feel better :)"

  print()
  print(output)
  print()


