# track_multiple_repos_traffic

Demo of some code to track the traffic on multiple repos beyond the 15 days limit


> this repo draws a lot of inspiration from the [repository-traffic-action](https://github.com/sangonzal/repository-traffic-action). We encourage you to have a look at it if this sort of things are interesting to you.


Using github actions, we execute a python script (`scan_multiple_github_repo_traffic.py`) which looks at the github repositories listed in `repos_to_watch.txt`.

The traffic information is stored and updated in the `traffic/` folder.



To be able to access the traffic information, we have defined a "TRAFFIC_ACTION_TOKEN" secret on this repo which contains a Personal Access Token with the requisite accesses to the tracked repositories (for a fine-grained PAT, you need to allow permission for "administration", read-only is enough).

