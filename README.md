how to add secret SPAMMIE_KEYTAB_FILE
what's the teamlab secret

Rao: 
1. stage messagecreator VIP switch
2. keytab secret

-------

cream cheese!

curl -H "Authorization: Bearer 15488-P6MW8ea5fSdZgwl7Jw" -H "Content-Type: application/json" --data '{"body": "edited body"}' -X PATCH "https://elb.c1.stage-central-1.mesos.yammer.com:10382/api/v2/messages/114039454"


adjust staging breakerbox value for 

==========================================

Handover:

1. Azure migration: MC & Spammie finish-up
2. Rich Text Spec


Messages:
1. how is the cache setup inside the Java service for Workfeed to use?

how many write/read requests do we have these days?
- POST /api/v1/messages
- POST/GET /api/v2 (Hydrant)

my guess is that Messages service has memcached client that talks to WF's memcached cluster to invalidate/update(?) cache.
Does Hydrant benefit from this cache at all?
Can we slowly remove cache and look at the effect?

Goal for this week: 

understand the whole workflow of Dockerization
- who reads .release_settings.yml
- how's metrics being sent to wavefront
- how's logs being sent to lens
- how's breakerbox metrics being sent
- WTF is tenacity wrapper