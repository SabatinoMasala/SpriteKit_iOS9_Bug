# SpriteKit > SKSpriteNode Major Bug in iOS9

## Case #1 

This repository has been created to highlight a major SpriteKit/SKSpriteNode Bug in iOS 9
when loading an SKSpriteNode through the following line :

let sprite = SKSpriteNode(imageNamed:"Spaceship_1")

The image "Spaceship_1" is part of Assets.xcassets.
The bug occurs when it is NOT a universal image, so I have made it an iPhone-only image.

The code behaves correctly under freshly resetted iPhone 6s, iPhone 6, iPhone 5s simulators.
It does NOT under freshly resetted iPhone 5 and 4s simulators.

Xcode seems to find the image, because it does not output any warning, and the image is an empty image rather than a red X in a white square.

## Case #2

Not working yet, but the same code in my game Trolls vs Leprechaun does not always work.
