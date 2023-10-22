<p align="center">
  <a href="https://fujurt.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dmklon1yi/image/upload/v1697986734/Fujurt/xiknoc16uit2bjyv7n51.png">
      <img alt="Fujurt logo" src="https://res.cloudinary.com/dmklon1yi/image/upload/v1697986734/Fujurt/xiknoc16uit2bjyv7n51.png">
    </picture>
  </a>
</p>

<h3 align="center">Publish Github Wiki Action</h3>
<p align="center">This action helps syncs your project's documentation with your project's Github Wiki.</p>

-------

## Usage

Add the following workflow as a step in your existing workflow or a new one, replacing `user_name` and `user_email` with your account/bot information.

```yml
- name: Publish Github Wiki
  uses: fujurt/publish-github-wiki-action@v1.0
  with:
    user_name: John Smith
    user_email: john_smith@email.com
    user_access_token: ${{ secrets.USER_ACCESS_TOKEN }}
```

<!-- TODO: Allow users to customize the wiki directory folder -->
This workflow will synchronize the `.github/wiki` folder with your project's Github Wiki.

## Setup

To use this workflow, your project must have the following:

- The Github Wiki must be enabled and initialized.
- A valid Personal Access Token must be provided to the workflow.

Below are steps to ensure proper setup:

1. **Enable the Wiki feature**

   You can enable the Wiki through your project's "Settings" tab.

   ![Wiki Feature in Settings](https://user-images.githubusercontent.com/34730459/162665798-a6464c67-c74a-427e-9221-4df8310fe9cb.png)

2. **Create at least one Wiki Page in the "Wiki" tab**

   This is required to initialize the project's Wiki repository.

   ![Create Wiki Page](https://user-images.githubusercontent.com/34730459/162666191-5f8cf77b-925f-4bec-b3b9-4ae4996444a9.png)

3. **Create a Personal Access Token with the `repo` scope enabled**

   Navigate to the [Personal Access Token](https://github.com/settings/tokens) page under the "Developer Settings" in your **user/bot account** "Settings" and generate the token.

   ![Generate Token](https://user-images.githubusercontent.com/34730459/162668740-b0ef45da-0985-4953-80c7-c60c35f5aefa.png)

   Ensure your token is copied/saved for the next step.

4. **Add the created Personal Access Token as a secret**

   Navigate to "Secrets > Actions" under the projects "Settings" tab to add a secret.

   ![Add new secret](https://user-images.githubusercontent.com/34730459/162669143-6fe258ad-b058-48a1-9c7b-dcbb1ecd0452.png)

## License

This project is Copyright (c) 2023 and onwards Fujurt or Fujurt X. It is free software
and may be redistributed under the terms specified in the [LICENSE] file.

[LICENSE]: /LICENSE

## About

<a href="https://fujurt.com/">
  <picture style="width: 128px; margin-bottom: 1rem;">
    <source media="(prefers-color-scheme: dark)" srcset="https://res.cloudinary.com/dmklon1yi/image/upload/v1697986734/Fujurt/xiknoc16uit2bjyv7n51.png">
    <img alt="Fujurt logo" src="https://res.cloudinary.com/dmklon1yi/image/upload/v1697986734/Fujurt/xiknoc16uit2bjyv7n51.png" style="width: 128px; margin-bottom: 1rem;">
  </picture>
</a>

This project is maintained and funded by Fujurt.

We love open source and do our part in sharing our work with the community!
See [our other projects][community] or [hire our team][hire] to help build your product.

[community]: https://github.com/fujurt
[hire]: https://fujurt.com/
