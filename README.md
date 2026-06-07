from flask import Flask

app = Flask(__name__)

@app.route("/")
def home():
    return """
    <h1>Mizgir</h1>
    <p>Добро пожаловать в Mizgir!</p>
    """

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000)
