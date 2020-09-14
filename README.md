# XcodeSnippets

## 1. SwiftUI preview snippet (Xcode 11 or later)

     import SwiftUI

     struct <# Controller name #>Provider : PreviewProvider {
        static var previews: some View {
           ContainerView().edgesIgnoringSafeArea(.all)
     }

      struct ContainerView: UIViewControllerRepresentable {
    
        let viewController = <# Controller name #>()
    
        func makeUIViewController(context: Context) -> UIViewController {
            return viewController
        }
    
        func updateUIViewController(_ uiViewController: UIViewController, context: Context) {
        
        }
      }
   }

To use run in terminal 

open _~/Library/Developer/Xcode/UserData/CodeSnippets_

copy files from Snippets folder

reopen Xcode

Start typing "swiftuipreview" in code **after** implementing your ViewController class, **not inside**.
