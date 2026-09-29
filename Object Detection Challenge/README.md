In the Object Detection Challenge, teams must train an object detection model to classify differently colored shapes and perform relevant movements

There are three colors, green, yellow, and purple, and three shapes, circles, triangles, and squares, making nine possible combinations. Teams are provided a dataset containing 4500 images and their respecitve YOLO V8 labels to train their model. Teams are allowed to use other object detection models if they wish, though new labels must be generated to fit the specified model

The object detection model must be able to detect and draw a bounding box around all nine colored shape combinations, but must only provide movement commands to the drone in the case of circles. The following are the respective movement commands for each circle:

Green Circle: move up 50, move down 100, move up 50

Yellow Circle: move forward 50, move back 100, move forward 50

Purple Circle: move right 50, move left 100, move right 50

The drone is only allowed to do each colored circle movement once, simply drawing the bounding box and not moving when seeing the same colored circle later on. Once all colored circle movements have been completed, the drone must move up 20 and then do a backflip (NOTE: the drone musth have more than 50% battery to do the flip)

Judges will show different shapes on at a time to test the model's classification precision. Scoring will be done both on the model's ability to correctly detect and classify each colored shape, as well as the drone's ability to perform relevant movements related to each colored circle and after all three colored circles have been detected
