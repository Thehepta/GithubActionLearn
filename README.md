first commit

workflows中定义了一个 webhook-1 事件，通过下面这个请求可以直接触发他，注意替换一些仓库，key，事件这些

curl -X POST https://api.github.com/repos/Thehepta/GithubActionLearn/dispatches \
    -H "Accept: application/vnd.github.everest-preview+json" \
    -H "Authorization: token ghp_xxxx" \
    --data '{"event_type": "webhook-1"}'
