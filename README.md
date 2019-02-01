# Blackjack-Implementation-using-Reinforcement-Learning

- Blackjack is a card game where the player plays against the dealer. The game is as follows:
1. The game starts off with 2 cards each, where only one is open for the other person to view and one is closed. 
2. The player can hit (1) and continue to be dealt cards. 
3. He/she can stick (0) when he/she thinks that the sum of all his cards is close but less than 21. 
4. If the sum is greater than 21, he goes bust and the dealer wins. 
5. Once the player sticks, the dealer is now dealt cards until the sum of the dealer's cards is greater than or equal to 17. 
6. If the sum of the dealer's cards is greater than 21, the dealer goes bust and the player wins. 
7. At the end, if both do not go bust, the sum of the cards is compared and the one closest to 21 wins.

## The reinforcement learning problem here is the agent (player) who is trying to maximize his rewards (wins)

The agent is the player

The environment is OpenAI's Gym (Blackjack-v0)

The state is a tuple of 3 values: (Sum of players cards, the value of the dealer's showing card, player's usuable ace binary)

The reward is -1 if the player loses, 0 if draw, 1 if the player wins 

In the python implementation of this problem, this is modelled as a Monte-Carlo problem.
