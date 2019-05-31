
## Matt Henley's Gitfolio Page 

![Gitfolio](https://github.com/mattbhenley/Images/blob/master/gitfolio.PNG)

### Let's Install

Install gitfolio

```sh
npm i gitfolio -g
```

### Let's Build

```sh
gitfolio build <username>
```
`<username>` is your username on github. This will build your website using your GitHub username and put it in the `/dist` folder.

To run your website use `run` command

```sh
gitfolio run
```

🎉 Congrats, you're done! 


### Let's Customize

#### Forks

To include forks on your personal website just provide `-f` or `--fork` argument while building

```sh
$ gitfolio build <username> -f
```

#### Sorting Repos

To sort repos provide `--sort [sortBy]` argument while building. Where `[sortBy]` can be `star`, `created`, `updated`, `pushed`,`full_name`. Default: `created`

```sh
$ gitfolio build <username> --sort star
```

#### Ordering Repos

To order the sorted repos provide `--order [orderBy]` argument while building. Where `[orderBy]` can be `asc` or `desc`. Default: `asc`

```sh
$ gitfolio build <username> --sort star --order desc
```

#### Customize Themes

Themes are specified using the `--theme [theme-name]` flag when running the `build` command. The available themes are

* `light`
* `dark`
> TODO: Add more themes

For example, the following command will build the website with the dark theme
```sh
$ gitfolio build <username> --theme dark
```

#### Customize background image

To customize the background image just provide `--background [url]` argument while building

```sh
$ gitfolio build <username> --background https://images.unsplash.com/photo-1557277770-baf0ca74f908?w=1634
```

You could also add in your custom CSS inside `index.css` to give it a more personal feel.


### Let's Publish

 Push the files inside`/dist` folder to repo you created! 

Go To `username.github.io` your site should be up!!


### Updating

To update your info, simply run

```sh
$ gitfolio update
```
This will update your info and your repository info.

To Update background or theme you need to run `build` command again.
