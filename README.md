# Monopoly recognition
[![Python 3.8](https://img.shields.io/badge/Python%20-3.8-informational)](https://www.python.org/downloads/release/python-3816/)
![](https://github.com/alessandro1802/board-game-recognition/blob/main/demo.gif)
## Technique and approach
The project is based on classic *Computer Vision* techniques, hence, **no** *Neural Networks* are involved.  
The notebook `recognize` (executable code) is self-explanatory, so the detailed description of how everything works is present there.

## Set-up
1. After cloning the repository, create a `Python 3.8` virtual environment: 
```bash
python3.8 -m venv venv
```
2. Activate it: 
```bash
source vevn/bin/activate 
```
3. Install the required libraries: 
```bash
pip install -r requirements.txt
```

## Data-set
There are 3 levels of difficulty:

### Easy
1. The view is nearly vertical.
2. The light is very good.
3. There are almost no shadows.
4. The board is straightly positioned.
5. The pawns are never covered.
6. Less moves.

### Medium
1. The view is nearly vertical.
2. Quite bad light.
3. Soft shadows are presents.
4. The board may be tilted.
5. The pawn may be partially covered by fingers.
6. More moves.

### Hard
1. Angled view.
2. Awful light.
3. Extreme shadows.
4. The board may be tilted.
5. The pawn may be heavily covered by fingers.
6. More moves.

## File-structure
1. `data/`

	a) input videos separated by difficulty level
	
	b) `train/` contains heuristic templates
	
2. `output/`

	a) rendered videos siparated by difficulty level
	
	b) `intemediate/` contains output demos obtained while processing
	
3.  Project files

	a) `recognize.ipynb` is the notebook with how it works explanations and code
	
	b) `requirements.txt` is the list of dependencies
	
