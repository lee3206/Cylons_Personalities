# Team 
Lee Taber
Kevin Weatherwax
Sean Fernandes

# Cylons_Personalities
Detect Robits from Photos and Personality From Text
  
  This does maybe one of those


# To Detect Personality
Run the personality.ipynb as a google colab.
(This isn't currently working, will continue to work on it)

# To Detect Robits
Create a jpyitder environment, and run the following commands:

~~~bash
pip install --upgrade "tensorflow==1.7.*"

git clone https://github.com/lee3206/Cylons_Personalities/tree/master/Cylon%20detector

cd wherever you cloned that\"cylon detector"

python -m scripts.label_image --graph=tf_files/retrained_graph.pb --image=tf_files/42b.jpg
~~~

You should get a return that the person is 99% human.

Now try this

~~~bash
python -m scripts.label_image --graph=tf_files/retrained_graph.pb --image=tf_files/11_nao-humanoid.jpg
~~~

You should get a return that the robot is 100% robotic

Add your own pictures to that directory to see if they are cylons or not
