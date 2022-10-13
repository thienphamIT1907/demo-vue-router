<template>
  <div class="container">
    <div class="avatar">
      <img :src="item.avatar_url" alt="avt"/>
    </div>
    <div class="basic-info">
      <p>{{item.login}}</p>
      <p>{{item.id}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'GithubItem',
  data() {
    return {
      item: {
        "login": "PeterDaveHello",
        "id": 3691490,
        "node_id": "MDQ6VXNlcjM2OTE0OTA=",
        "avatar_url": "https://avatars.githubusercontent.com/u/3691490?v=4",
        "gravatar_id": "",
        "url": "https://api.github.com/users/PeterDaveHello",
        "html_url": "https://github.com/PeterDaveHello",
        "followers_url": "https://api.github.com/users/PeterDaveHello/followers",
        "following_url": "https://api.github.com/users/PeterDaveHello/following{/other_user}",
        "gists_url": "https://api.github.com/users/PeterDaveHello/gists{/gist_id}",
        "starred_url": "https://api.github.com/users/PeterDaveHello/starred{/owner}{/repo}",
        "subscriptions_url": "https://api.github.com/users/PeterDaveHello/subscriptions",
        "organizations_url": "https://api.github.com/users/PeterDaveHello/orgs",
        "repos_url": "https://api.github.com/users/PeterDaveHello/repos",
        "events_url": "https://api.github.com/users/PeterDaveHello/events{/privacy}",
        "received_events_url": "https://api.github.com/users/PeterDaveHello/received_events",
        "type": "User",
        "site_admin": false,
        "score": 1.0
      },
    }
  },
}
</script>

<style scoped>
  .container {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 10px;
    background: #43b784;
    border-radius: 12px;
    font-size: 23px;
    width: 100%;
    max-width: 450px;
    transition: all 0.2s;
  }

  .container:hover {
    cursor: pointer;
    transform: scale(1.1)
  }

  .avatar {
    width: 100px;
    height: 100px;
  }

  .avatar > img {
    width: 100%;
    height: 100%;
    border-radius: 100%;
  }

  .basic-info {
    display: flex;
    justify-content: start;
    align-items: center;
    flex-direction: column;
    margin-left: 20px;
  }

  .basic-info > p {
    text-align: left;
    width: 100%;
  }
</style>