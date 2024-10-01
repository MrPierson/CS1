
# Basic Python Style Guide

## 1. Variable Naming
- **Use meaningful names**: Variable names should describe what the variable is storing.
  ```python
  # Good
  player_name = "Alice"
  
  # Bad
  pn = "Alice"
  ```
  
- **Use lowercase letters with underscores**: Separate words with underscores (`snake_case`).
  ```python
  player_score = 0
  game_level = 1
  ```

- **Avoid single letter variable names** unless it's a simple counter or loop variable.
  ```python
  # Good
  for i in range(10):
      print(i)
  
  # Bad
  x = 100  # What does 'x' mean?
  ```

## 2. Functions
- **Function names should be descriptive and use `snake_case`.**
  ```python
  def calculate_score(player_score, bonus):
      return player_score + bonus
  ```

- **Keep functions short and focused on one task**. A function should "do one thing" clearly.
  ```python
  def display_welcome_message():
      print("Welcome to the game!")
  ```

- **Use comments to explain what the function does**, especially if it's not immediately clear.
  ```python
  def get_user_input():
      # Ask the user for input and return it as an integer
      user_input = input("Enter a number: ")
      return int(user_input)
  ```

## 3. Lists
- **Use plural names for lists** to show that they hold multiple items.
  ```python
  players = ["Alice", "Bob", "Charlie"]
  ```

- **Avoid hardcoding list indexes**. Use loops when accessing elements.
  ```python
  # Good
  for player in players:
      print(player)

  # Bad
  print(players[0])
  print(players[1])
  print(players[2])
  ```

## 4. Indentation
- **Use 4 spaces per indent level**. Never use tabs or a mix of spaces and tabs. Most code editors handle this automatically.
  ```python
  def start_game():
      print("Game starting...")
      player_score = 0
      return player_score
  ```

## 5. Print and Input
- **Keep `print` statements simple and clear**. Print only the necessary information.
  ```python
  # Good
  print("Player score:", player_score)
  
  # Bad
  print("The score of the player is currently this: ", player_score)
  ```

- **Use `input` in a way that helps the user understand what they need to do.**
  ```python
  # Good
  name = input("Enter your name: ")

  # Bad
  name = input()
  ```

## 6. Comments
- **Use comments to explain why you are doing something**, not what the code does. Write comments above the code they describe.
  ```python
  # Calculate the player's final score with the bonus
  final_score = player_score + bonus
  ```

- **Don't over-comment**. If your code is clear, you don't need a comment for everything.
  ```python
  # Bad
  player_name = "Alice"  # Set player name to Alice
  ```

## 7. Code Layout
- **Leave a blank line between different sections of your code** for better readability.
  ```python
  def start_game():
      print("Welcome!")
      
      player_name = input("Enter your name: ")
      return player_name
  ```

- **Group related code together**. Keep related logic, like variable declarations or function calls, in the same area.

## 8. Consistency
- **Be consistent** with your style. If you choose to name variables with `snake_case`, keep that style throughout the program.
  ```python
  # Consistent
  player_name = "Alice"
  player_score = 100
  
  # Inconsistent (bad)
  playerName = "Alice"
  player_score = 100
  ```
