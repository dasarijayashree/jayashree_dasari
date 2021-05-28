def build_model(hp):

model keras.Sequential([

keras.layers.Conv2D(

filters-hp.Int('com_1_filter, min_value-32, max value=128, step-16),

kernel_size-hp.Choice( conv_1_kernel", values= [3,5]), activation='relu',

input shape-(28,28,1)

keras.layers.Conv2D(

filters=hp.Int('com_2_filter, min_value-32, max_value-64, step-16), kernel_size=hp.Choice('conv 2 kernel", values = [3,5]),

activation='relu'

), keras.layers.Flatten(),

keras.layers.Dense(

units-hp.Int('dense 1 units, min_value-32, max value-128, step-16),

activation='relu'

keras.layers.Dense(10, activation='softmax')output layer
