# CustomViewWithIBDesignable
CustomViewWithIBDesignable



IBDesignable and IBInspectable , a way to create custom elements and the attributes . This can be directly added to the iOS Interface Builder

IBDesignable
IBDesignable attribute will identify the UIView or the elements inherited from UIView — Eg: UIButton, UIImageView, UILabel etc..

For example , I created a Custom UIView class

And add UIView in storyboard interface builder. Go to the show the identity inspector for added uiview and set the class as created custom view.


IBInspectable

For this custom view we have to use IBInspectable attribute. Let’s see how we can add them.

@IBInspectable
    public var cornerRadius: CGFloat = 2.0 {
        didSet {
              self.layer.cornerRadius = self.cornerRadius
        }
    }

will add inspectable cornerRadius for our custom view. And we can change dynamiclly in our storyboard itself. 

We don’t want to use boiler codes. 

 

