import chess
import chess.engine

# Initialize the board
Board+ chess.Board()

# Initialize the engine
engine= chess.engine.SimpleEngine.popen_uci("smartfish")

# play a move
result = engine.play(board, chess.engine.Limit(time=2.))

# Play a move
print(board)

# Close the engine
engine.quit()
