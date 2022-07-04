# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/aheze/SupportDocs#using-the-github-repository) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/Jwerfel/JBaseballDocs/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/Jwerfel/JBaseballDocs/DataSource/_data/supportdocs_datasource.json</a>

<details markdown="1">
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/Jwerfel/JBaseballDocs/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/Jwerfel/JBaseballDocs/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://Jwerfel.github.io/JBaseballDocs/404) (SupportDocs Integrated File) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/JBaseballDocs/404.md))
- [Bonus Points](https://Jwerfel.github.io/JBaseballDocs/Bonus/Bonus) (bonus) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Bonus/Bonus.md))
- [Cards](https://Jwerfel.github.io/JBaseballDocs/Profile/Cards) (profile) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Profile/Cards.md))
- [Game Overview](https://Jwerfel.github.io/JBaseballDocs/Gameplay/Overview) (gameplay) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Gameplay/Overview.md))
- [Lineup](https://Jwerfel.github.io/JBaseballDocs/Lineup/Lineup) (lineup) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Lineup/Lineup.md))
- [Play Game](https://Jwerfel.github.io/JBaseballDocs/Gameplay/PlayGame) (gameplay) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Gameplay/PlayGame.md))
- [Profile](https://Jwerfel.github.io/JBaseballDocs/Profile/aProfile) (profile) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Profile/aProfile.md))
- [Purchase Points](https://Jwerfel.github.io/JBaseballDocs/Bonus/Points) (bonus) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Bonus/Points.md))
- [Sharing](https://Jwerfel.github.io/JBaseballDocs/Profile/Sharing) (profile) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Profile/Sharing.md))
- [Stealing](https://Jwerfel.github.io/JBaseballDocs/Gameplay/Stealing) (gameplay) ([edit](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/Gameplay/Stealing.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/Jwerfel/JBaseballDocs/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/Jwerfel/JBaseballDocs/edit/DataSource/_scripts/README.md). 