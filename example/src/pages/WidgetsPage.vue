<template>
  <div>
    <h5>Info Box</h5>
    <b-row class="mb-4">
      <b-col>
        <a-lte-info-box :icon="['far', 'envelope']" header="Messages" icon-variant="info">1,410</a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'flag']" header="Bookmarks" icon-variant="success">410</a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'copy']" header="Uploads" icon-variant="warning">13,648</a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'star']" header="Likes" icon-variant="danger">93,139</a-lte-info-box>
      </b-col>
    </b-row>

    <h5>Info Box With <code>&lt;a-lte-info-box variant="*"&gt;</code></h5>
    <b-row class="mb-4">
      <b-col>
        <a-lte-info-box :icon="['far', 'bookmark']" header="Bookmarks" variant="info">
          41,410
          <b-progress :value="30" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'thumbs-up']" header="Likes" variant="success">
          41,410
          <b-progress :value="50" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'calendar-alt']" header="Events" variant="warning">
          41,410
          <b-progress :value="70" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'comments']" header="Comments" variant="danger">
          41,410
          <b-progress :value="80" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
    </b-row>

    <h5>Info Box WIth <code>&lt;a-lte-info-box variant="*" gradient&gt;</code></h5>
    <b-row class="mb-4">
      <b-col>
        <a-lte-info-box :icon="['far', 'bookmark']" header="Bookmarks" variant="info" gradient>
          41,410
          <b-progress :value="10" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'thumbs-up']" header="Likes" variant="success" gradient>
          41,410
          <b-progress :value="25" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'calendar-alt']" header="Events" variant="warning" gradient>
          41,410
          <b-progress :value="45" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
      <b-col>
        <a-lte-info-box :icon="['far', 'comments']" header="Comments" variant="danger" gradient>
          41,410
          <b-progress :value="85" />
          70% Increase in 30 Days
        </a-lte-info-box>
      </b-col>
    </b-row>

    <h5>Small Box</h5>
    <b-row class="mb-4">
      <b-col>
        <a-lte-small-box variant="info" icon="shopping-cart" to="#">
          <h3>150</h3>
          <p>New orders</p>
          <template slot="footer">
            More info
            <font-awesome-icon icon="arrow-alt-circle-right" />
          </template>
        </a-lte-small-box>
      </b-col>
      <b-col>
        <a-lte-small-box variant="success" icon="chart-bar" footer="It's not a link">
          <h3>53<sup>%</sup></h3>
          <p>Bounce Rate</p>
        </a-lte-small-box>
      </b-col>
      <b-col>
        <a-lte-small-box variant="warning" icon="user-plus" to="#">
          <h3>44</h3>
          <p>User Registrations</p>
          <template slot="footer">
            More info
            <font-awesome-icon icon="arrow-alt-circle-right" />
          </template>
        </a-lte-small-box>
      </b-col>
      <b-col>
        <a-lte-small-box variant="danger" icon="chart-pie" to="#" footer="More info">
          <h3>65</h3>
          <p>Unique Visitors</p>
        </a-lte-small-box>
      </b-col>
    </b-row>

    <h5>Cards</h5>
    <b-row class="mb-4">
      <b-col>
        <b-card no-body>
          <b-card-header>
            <a-lte-card-title>Expandable</a-lte-card-title>
            <a-lte-card-tools>
              <b-button v-b-toggle.card-1 variant="tool" type="button">
                <font-awesome-icon icon="plus" />
              </b-button>
            </a-lte-card-tools>
          </b-card-header>
          <b-collapse id="card-1">
            <b-card-body>
              The body of the card
            </b-card-body>
          </b-collapse>
        </b-card>
      </b-col>
      <b-col>
        <b-collapse id="card-2" visible>
          <b-card no-body>
            <b-card-header header-bg-variant="success">
              <a-lte-card-title>Removable</a-lte-card-title>
              <a-lte-card-tools>
                <b-button v-b-toggle.card-2 variant="tool" type="button">
                  <font-awesome-icon icon="times" />
                </b-button>
              </a-lte-card-tools>
            </b-card-header>
            <b-card-body>
              The body of the card
            </b-card-body>
          </b-card>
        </b-collapse>
      </b-col>
      <b-col>
        <b-card no-body>
          <b-card-header header-bg-variant="warning">
            <a-lte-card-title>Expandable</a-lte-card-title>
            <a-lte-card-tools>
              <b-button v-b-toggle.card-3 variant="tool" type="button">
                <font-awesome-icon icon="minus" />
              </b-button>
            </a-lte-card-tools>
          </b-card-header>
          <b-collapse id="card-3">
            <b-card-body>
              The body of the card
            </b-card-body>
          </b-collapse>
        </b-card>
      </b-col>
      <b-col>
        <b-card no-body>
          <b-card-header header-bg-variant="danger">
            <a-lte-card-title>Loading state</a-lte-card-title>
          </b-card-header>
          <b-card-body>
            The body of the card
          </b-card-body>
          <a-lte-card-overlay>
            <font-awesome-icon icon="sync-alt" size="2x" spin />
          </a-lte-card-overlay>
        </b-card>
      </b-col>
    </b-row>
  </div>
</template>
