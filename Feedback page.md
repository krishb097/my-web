<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Website Feedback Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1740&q=80');
            background-size: cover;
            background-position: center;
            padding: 20px;
            color: #000;
        }

        .feedback-form {
            background-color: transparent;
            padding: 25px;
            border-radius: 8px;
            max-width: 600px;
            margin: auto;
            box-shadow: 0 0 15px rgb(10, 0, 0);
        }

        .feedback-form h2 {
            text-align: center;
            text-decoration: underline;
        }

        label {
            display: block;
            margin-top: 15px;
            font-weight: bold;
            transition: color 0.2s ease;
        }

        label:hover {
            color: #4CAF50;
            cursor: pointer;
        }

        input[type="text"],
        textarea,
        select {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #000;
            border-radius: 4px;
            resize: vertical;
            transition: all 0.3s ease;
        }

        input[type="text"]:hover,
        textarea:hover,
        select:hover {
            border-color: #4CAF50;
            background-color: #f9fff9;
            transform: scale(1.03);
        }

        input[type="radio"] {
            margin-right: 10px;
            transition: transform 0.2s ease;
        }

        input[type="radio"]:hover {
            transform: scale(1.1);
            cursor: pointer;
        }

        .rating-group {
            display: flex;
            justify-content: space-between;
            margin-top: 5px;
        }

        .submit-btn {
            background-color: rgb(8, 202, 8);
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            margin-top: 20px;
            cursor: pointer;
            width: 100%;
            transition: all 0.3s ease;
        }

        .submit-btn:hover {
            background-color: transparent;
            color: black;
            border: 1px solid black;
            transform: scale(1.05);
        }
    </style>
</head>
<body>

<div class="feedback-form">
    <h2>Website Feedback Form</h2>
    <form action="feed.html" method="post">
        <label>1. How satisfied are you with your experience?</label>
        <label><input type="radio" name="satisfaction" value="Very satisfied"> Very satisfied</label>
        <label><input type="radio" name="satisfaction" value="Satisfied"> Satisfied</label>
        <label><input type="radio" name="satisfaction" value="Neutral"> Neutral</label>
        <label><input type="radio" name="satisfaction" value="Dissatisfied"> Dissatisfied</label>
        <label><input type="radio" name="satisfaction" value="Very dissatisfied"> Very dissatisfied</label>

        <label for="purpose">2. What was the purpose of your visit today?</label>
        <input type="text" id="purpose" name="purpose">

        <label for="found">3. Were you able to find what you were looking for?</label>
        <select id="found" name="found">
            <option value="Yes">Yes</option>
            <option value="Partially">Partially</option>
            <option value="No">No</option>
        </select>

        <label for="navigation">4. How easy was it to navigate our website?</label>
        <select id="navigation" name="navigation">
            <option value="Very easy">Very easy</option>
            <option value="Easy">Easy</option>
            <option value="Neutral">Neutral</option>
            <option value="Difficult">Difficult</option>
            <option value="Very difficult">Very difficult</option>
        </select>

        <label>5. How would you rate the following (1 = Poor, 5 = Excellent)?</label>

        <label>Website Design</label>
        <div class="rating-group">
            <label><input type="radio" name="design" value="1">1</label>
            <label><input type="radio" name="design" value="2">2</label>
            <label><input type="radio" name="design" value="3">3</label>
            <label><input type="radio" name="design" value="4">4</label>
            <label><input type="radio" name="design" value="5">5</label>
        </div>

        <label>Content Quality</label>
        <div class="rating-group">
            <label><input type="radio" name="content" value="1">1</label>
            <label><input type="radio" name="content" value="2">2</label>
            <label><input type="radio" name="content" value="3">3</label>
            <label><input type="radio" name="content" value="4">4</label>
            <label><input type="radio" name="content" value="5">5</label>
        </div>

        <label>Page Load Speed</label>
        <div class="rating-group">
            <label><input type="radio" name="speed" value="1">1</label>
            <label><input type="radio" name="speed" value="2">2</label>
            <label><input type="radio" name="speed" value="3">3</label>
            <label><input type="radio" name="speed" value="4">4</label>
            <label><input type="radio" name="speed" value="5">5</label>
        </div>

        <label>Mobile Responsiveness</label>
        <div class="rating-group">
            <label><input type="radio" name="mobile" value="1">1</label>
            <label><input type="radio" name="mobile" value="2">2</label>
            <label><input type="radio" name="mobile" value="3">3</label>
            <label><input type="radio" name="mobile" value="4">4</label>
            <label><input type="radio" name="mobile" value="5">5</label>
        </div>

        <label for="errors">6. Did you encounter any errors or broken links?</label>
        <textarea id="errors" name="errors" rows="3" placeholder="If yes, please describe..."></textarea>

        <label for="likes">7. What do you like most about our website?</label>
        <textarea id="likes" name="likes" rows="3"></textarea>

        <label for="improve">8. What can we improve?</label>
        <textarea id="improve" name="improve" rows="3"></textarea>

        <label for="recommend">9. Would you recommend our website to others?</label>
        <select id="recommend" name="recommend">
            <option value="Yes">Yes</option>
            <option value="No">No</option>
            <option value="Maybe">Maybe</option>
        </select>

        <label for="comments">10. Additional comments or suggestions:</label>
        <textarea id="comments" name="comments" rows="4"></textarea>

        <button type="submit" class="submit-btn">Submit Feedback</button>
    </form>
</div>

</body>
</html>
