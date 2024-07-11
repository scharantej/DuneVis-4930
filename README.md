## Flask Application Design

## HTML Files

- **index.html**: This will serve as the main landing page for the project. It will include the core content and visual elements that showcase the game's features and appeal to potential players.

## Routes

- **/**: This route will render the **index.html** template.

## Code

### app.py
```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def index():
    return render_template('index.html')

if __name__ == "__main__":
    app.run(debug=True)
```