the message passd to the AWS Firehose (and probably all other) node to:
* MUST: msg.Record.Data = [JSON String]  <= NOT JSON object of the data to be sent to AWS
* CAN:  msg.DeliveryStreamName = "FIREHOSE_STREAM_NAME" (otherwise the node param will override the config)
* CAN:  msg.AWSConfig={ accessKeyId: "ACCESS KEY", secretAccessKey:"SECRET KEY", region:"Region" }