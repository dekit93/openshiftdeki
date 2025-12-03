
import random
from flask import Flask

app = Flask(__name__)

@app.route("/")
def generate_teams():
    teams = ["Brazil", "Argentina", "France", "Germany", "Spain", "England", "Italy", "Portugal"]
    groups = ["A", "B", "C", "D"]
    random.shuffle(teams)
    result = [f"{team} -> Group {groups[i % len(groups)]}" for i, team in enumerate(teams)]
    return "<br>".join(result)

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=8080)
