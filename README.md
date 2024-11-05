# Project overview
...

# Installation

1. **Clone the repository**:

```bash
git clone https://github.com/YourUsername/repository_name.git
```

2. **Install UV**

If you're a MacOS/Linux user type:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

If you're a Windows user open an Anaconda Powershell Prompt and type :

```bash
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

3. **Create an environment**

```bash
uv venv 
```

3. **Activate the environment**

If you're a MacOS/Linux user type (if you're using a bash shell):

```bash
source ./venv/bin/activate
```

If you're a MacOS/Linux user type (if you're using a csh/tcsh shell):

```bash
source ./venv/bin/activate.csh
```

If you're a Windows user type:

```bash
.\venv\Scripts\activate
```

4. **Install dependencies**:

```bash
uv pip install -r requirements.txt
```

# Questions 
...

# Dataset 
...
For this project, we used "Top 1500 games on steam by revenue 09-09-2024" dataset which can be find on this link: https://www.kaggle.com/datasets/alicemtopcu/top-1500-games-on-steam-by-revenue-09-09-2024?resource=download

As this dataset lack some information that we were looking for, we also used Steam API and added several columns, by looping through each steamID (which is unique for every game)/

## Main dataset issues

- Missing information in the main dataset
- Finding other sources to complete the dataset

## Solutions for the dataset issues
- Using Steam API to add the required information to the dataset.

# Hypothesises:
- Is there a correlation between the release time (holidays, sales) and revenue?
- Examining the correlation between genre and revenue/
- Games with high reviewScores and positive reviewScore generate higher revenue.
- Genres with highest revenue
- Do more expensive games have higher rating?

# Conclussions and findings:
...
- The price of the game and its review score don't have any meaningful correlation with each other.
- The top 5 highest grossing games released during the Steam Sale have a mean revenue of $319,158.21, while the top 5 highest grossing games released outside of the Steam Sale have a mean revenue of $2,659,939.32. This is over 8 times higher.
The large gap in average revenue between these two groups suggests that release timing, specifically in relation to major sales events like the Steam Sale, has a substantial impact on a game's revenue performance. Games released during the Steam Sale seem to generate notably lower revenue on average compared to those released at other times
- 


# Next steps
- By using a dataset which contains the costs of producing games we can have a better look at profitability.
- The dataset can be merged with other gaming platforms to have a better overall view of game industry.
