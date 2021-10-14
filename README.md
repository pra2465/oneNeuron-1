# oneNeuron-1
oneNeuron@1|perceptron


# commands used -


```bash
git add . && git commit -m "docstring updated" && git push origin main
```

# Add URL-
[Git handbook](https://guides.github.com/introduction/git-handbook)

<a href="https://www.w3schools.com">Visit W3Schools.com!</a>

## Add image -
![sample Image](plots/or.png)

<img src="plots/or.png" alt="Girl in a jacket" width="500" height="600">

# python updated
``` python code
def main(data, modelname, plotname, eta, epochs):
    df = pd.DataFrame(data)
    print(df)
    X,y = prepare_data(df)
    model = Perceptron(eta=eta, epochs=epochs)
    model.fit(X, y)
    _ = model.total_loss()
    save_model(model, filename=modelname)
    save_plot(df, plotname, model)