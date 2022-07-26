# `TimeSpan` Usage Generalization

Time related settings &mdash;e.g. send port's retry interval, `WCF` channel's send timeout, or `SFTP` adapter's polling interval&mdash; are often, if not always, expressed in different time units &mdash;milliseconds, seconds, minutes&mdash; and rarely as plain `TimeSpan` values. `BizTalk.Factory`'s `Binding DSL` strives to standardize all these time related settings by surfacing them all as `TimeSpan`s through the `API`, therefore freeing the developer of having to remember the time unit in which he has to express an integer time value and performing the conversion to the right time unit for him.

Even when the unit in which is expressed the time is configurable too &mdash;for instance [`SFTP` Adapter][sftp-adapter-configuration]'s Receive Location `PollingInterval` and `PollingIntervalUnit`,&mdash; `BizTalk.Factory` surfaces these two properties as one single [Polling Interval][sftp-adapter-polling-interval], which, behind the scenes, is mapped to the two configurable properties of the actual configuration class.

<!-- links -->

[sftp-adapter-configuration]: https://docs.microsoft.com/en-us/biztalk/core/sftp-adapter#configure-the-receive-location
[sftp-adapter-polling-interval]: https://github.com/icraftsoftware/Be.Stateless.BizTalk.Dsl.Binding/blob/f635723e082b0a36d87331b0446347a5599c1d5a/src/Be.Stateless.BizTalk.Dsl.Binding/Dsl/Binding/Adapter/SftpAdapter.Inbound.cs#L98

<!--
cSpell:ignore
-->
