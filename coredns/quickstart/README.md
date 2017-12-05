# CoreDNS

## Run
* `coredns -conf /etc/coredns/Corefile -dns.port 1053`

## Test
* 查找 `www.example.org` 的 A 记录: `dig -p 1053 @localhost A www.example.org +noall +answer`
* 查找 `tt.example.org` 的 TXT 记录: `dig -p 1053 @localhost TXT tt.example.org +noall +answer`

## Refs
* <https://coredns.io/2017/07/24/quick-start/>
* <http://dmdgeeker.com/post/coredns-try/>
