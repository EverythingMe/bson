## This is an extraction (with a couple of minor modifications) of Youtube's BSON library that's part of Vitess.

See https://github.com/youtube/vitess/

It is extracted so it can be imported without having to vendor the entire Vitess tree, and for the following changes:

1. Fileds can have a struct tags, e.g `bson:"foo"` so overriding their struct names is possible.

2. Strings are encoded as BSON strings and not Binary (this means they have to be utf-8).


