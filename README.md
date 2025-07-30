# Advent_of_code_2023 - Jiveshwari's Solutions

# Progress
Completed till Day 3. Days 2 and 3 earned 2 stars each. Day 1 was incorrect due to edge cases I think. 

# Basic Thought Process and Explanation
Day 1: Trebuchet?!

Task: Extract first and last digits (or verbal digits) from each line, form a two-digit number, and sum them.
Approach: Scanned each line character by character, collecting digits or converting words (e.g., "one" to "1"). Combined first and last digits into a number (e.g., "1abc2" → 12).
Issue: Missed edge cases like overlapping words ("oneight" → 1, 8) and single-digit lines (e.g., "6" → 66).

Day 2: Cube Conundrum

Task: Part 1: Check if games are possible with 12 red, 13 green, 14 blue cubes; sum valid game IDs. Part 2: Find minimum cubes per game and sum their power (red * green * blue).
Approach: Parsed game sets, tracked cube counts per color. Part 1 checked against limits; Part 2 found max counts per color and calculated power.
Blocker: Parsing complex input strings was tricky; needed careful splitting of sets and counts.

Day 3: Gear Ratios

Task: Part 1: Sum numbers adjacent to symbols. Part 2: Sum gear ratios (* symbols with exactly two adjacent numbers, ratio = number1 * number2).
Approach: Scanned grid for numbers, checked adjacent positions for symbols (Part 1) or * with two numbers (Part 2). Used position tracking to identify valid numbers.
Blocker: Ensuring diagonal checks for adjacency were accurate required careful boundary handling.

# Room for Improvement

1. Input Management: Store inputs in separate files (e.g., input_day1.txt) for safety and readability.
2. Day 1: Use regular expressions with lookaheads to handle overlapping words (e.g., (?=(one|two|\d))) for cleaner code.

# Overall Experience
This was fun! Struggled with Day 1 edge cases but learned a lot. Created this repo to keep solving 2023 and maybe 2024 puzzles!
