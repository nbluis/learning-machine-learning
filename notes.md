Machine Learning
    Inputs a labels

    Whats is Machine Learning ?
        Field of study that gives computers the ability to learn without being explicitly programmed

    Supervised Learning
        Learns from data labeled with the "rights answers"

        Regression
            Infinite number of posibilities (a number, a value)
            - Predicts Numbers
            - Linear Regression

        Classification
            Small / finite / limited number of possibilities (m or n)
                - Classes or Categories
            - Predicts Categories

    Unsupervised Learning
        Find something interesting on unlabeled data

        - Clustering Algorithm
        - Anomaly Detection
        - Dimensionality Reduction


    - Recommender Systems
    - Reinforcement Learning


    Terminology:
        - Dataset
        - Training set
        - Predict
        - fit
        - x = input or feature or input feature
        - y = output or target or target output
        - m = total number of training examples
        - (x, y) = single training example = (10, 20)
        - (xⁱ, yⁱ) = ⁱ specific training example = row vector
        - y-hat = prediction result for a function f (hiphotesis). (xⁱ, yⁱ) <> f(i) <> ^y
        - function = model
        - parameters = variables you can adjust during training in order to improve the model (coefficients, weights)
        - J(w, b) = cost function = build the error between ^y - y
            - What the cost function does is, it measures the difference between the models predictions between actual true values to y
            - Linear regresion would try to find values for w and b, then make J(w, b) as small as possible
            - Goal: minimize J(w, b)
        - squared error cost function = J(w,b) = 1/2m * sum(^yⁱ - yⁱ)2
        - linear regression parameters minimize algorithm, gradient descent
        - learning rate or alpha or α = small posible number btw 0-1
        - derivative term = gradiant descendent math function
            - when derivative term is positive, the result w (or b) will be decrease
            - when derivative term is negative, the result w (or b) will be increase
        - gradient descent
            - used to calculate the linear regression parameters (w, b) to minimize meansure of error between prediction and the actual data
            - with fixed learning rate only can reach local minumum
            - batch gradiant descent - each step uses all the training samples instead of a subset
        - n = number of features
        - x₁, x₂, x₃ = feature index
        - ->w = w vector, ->x
        - ->w . ->x = product of w and x by index = (w₁ * x₁ + w₂ + x₂ + ... + wₙ + xₙ)
        - multiple linear regression = linear regression with multiple features
        - normal equation = alternative of linear regression
            - disvantages
                only for linear regression, no generalize to other learning algorithms
        - feature scaling = scaling features to turn him more comparable each other (orders of magnitude)
            - try to have features between small numbers close to zero - rescaling him when necessary
            - divide by maximum x = x / max([x])
                - produces smaller comparable numbers
            - mean normalization
                - (x₁ - μ₁) / (max - min)
                - x = x - avg([x]) / (max([x]) - min([x]))
                - produces x between -1 and 1
            - zero-score normalizaton
                - standard deviation
                - (x₁ - μ₁) / σ₁
                - x = (x - avg([x])) / std_dev(x, [x])
                - reduces the magnitudes but not normalizes deviations
        - learning curve = curve between iterations(x) and cost function J(y)
            - when the gratiant descent work properly, J decrease after every single iteration
            - when J increases, alpha is choose pooly (can be too large or in a local minimum)
            - whe the curve is not decreases, gradiant descent likely converged
        - automatic convergence test
            - if J(w,b) decreases by <= ε, declares it converged
            - dificult to find ε
        - feature engeneering = design new features by transforming or combining original features
        - polynomial regression = use polynomial functions to define features transformed from original that can represents non linear progressions on linear algorithm

