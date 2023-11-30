# Google Colab runtime on Fly GPUs

First deploy with:
```
fly apps create colab-gpu
fly deploy
```

Next, run `fly proxy 9000:8080`

Now, in [Colab](https://colab.research.google.com/), click the "Connect" button and select "Connect to local runtime...". Enter `http://127.0.0.1:9000` in the dialog that appears and click the "Connect" button. After this, you should now be connected to your local runtime.
