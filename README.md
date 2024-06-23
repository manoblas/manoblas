width, height = 800, 600
image = Image.new('RGB', (width, height), 'white')
draw = ImageDraw.Draw(image)
draw.rectangle([(0, 300), (800, 600)], fill='gray')  # Track
draw.rectangle([(0, 200), (800, 300)], fill='green')  # Grass
draw.ellipse([(50, 50), (150, 150)], fill='red', outline='black')  # Helmet
draw.rectangle([(50, 150), (150, 400)], fill='red', outline='black')  # Racing suit
draw.text((200, 50), "Lucas Silva", fill='black')
car_body = [(400, 450), (650, 500)]
car_windows = [(450, 460), (600, 490)]
draw.rectangle(car_body, fill='red', outline='black')
draw.rectangle(car_windows, fill='blue', outline='black')
for i in range(10, 800, 20):
    draw.ellipse([(i, 170), (i+10, 180)], fill='black')
