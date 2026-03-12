The "Trailblazer" Weather & Gear Validator
Build a tool that cross-references weather data with "Gear Recommendations" for hikers or campers.

The Goal: Write a script that hits the OpenWeatherMap API for a specific hiking trail. Based on the temp and condition returned, your script should validate an internal "Gear API" (which you can mock using pytest-mock) to ensure the correct equipment is suggested.

Python Tech Stack: Pytest, JSONSchema, responses (for mocking).

SDET Twist: Implement Contract Testing. Use Python to verify that the Weather API's response matches a specific schema. If the API adds a new field or changes a data type (e.g., temp changes from int to float), your test should catch the "contract breach."

Why it works: This mimics the "service-to-service" communication at Telus, where one team’s API change might break another team’s UI.
