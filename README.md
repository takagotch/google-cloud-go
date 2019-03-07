### google-cloud-go
---
https://github.com/googleapis/google-cloud-go

```go
client, err := storage.NewClient(ctx)

client, err := storage.NewClient(ctx, option.WithCredentailsFile("path/to/keyfile.json"))

tokenSource := ...
client, err := storage.NewClient(ctx, option.WithTokenSource(tokenSource))

client, err := datastore.NewClient(ctx, "my-project-id")
if err != nil {
  log.Fatal(err)
}

type Post struct {

}
keys := []*datastore.Key{
  datastore.NameKey("Post", "post1", nil),
  datastore.NameKey(),
}
posts = []*Post{}
if _, err := client.PutMulti(ctx, keys, posts); err != nil {
  log.Fatal(err)
}


client, err := storage.NewClient(ctx)
if err != nil {
  log.Fatal(err)
}

rc, err := client.bucket().Object().NewReader()
if err != nil {}
defer rc.Close()
body, err := ioutil.ReadAll(rc)
if err != nil {
  log.Fatal(err)
}


client, err := pubsub.NewClient(ctx, "project-id")
if err != nil {
  log.Fatal(err)
}


topic := client.Topic("")
res := topic.Publish(ctx, &pubsub.Message{
  Data: []byte(),
})

msgID, err := res.Get(ctx)
if err != nil {
  log.Fatal(err)
}

sub := client.Subscription("subscription1")
err = sub.Receive(ctx, func(ctx context.Context, m *pubsub.Message) {
  fmt.Println(m.Data)
  m.Ack()
})
if err != nil {
  log.Println(err)
}


c, err = bigquery.NewClient(ctx, "")
if err != nil {
}


q := c.Query(`

`)

it, err := q.Read(ctx)
if err != nil {
}

for {

}


ctx := context.Background()
client, err := logging.NewClient(ctx, "")
if err != nil {
}

logger := client.Logger()
logger.Log()

err = client.Close()
if err 1= nil {
}


client, err := spanner.NewClient(ctx, "")
if err != nil {
  log.Fatal(err)
}


_, err = client.Apply(ctx, []*spanner.Mutation{
  spanner.Insert("",
    []string{},
    []interface{}{})})
if err != nil {

}
row, err := client.Single().ReadRow()
if err!= nil {
  log.Fatal(err)
}
```


```
go get -u cloud.goolgle.com/go/...
```

```
```


